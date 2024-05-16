# Comparing `tmp/download-center-5.3.6.tar.gz` & `tmp/download-center-5.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download-center-5.3.6.tar", last modified: Wed May 15 02:45:36 2024, max compression
+gzip compressed data, was "download-center-5.3.7.tar", last modified: Thu May 16 10:00:07 2024, max compression
```

## Comparing `download-center-5.3.6.tar` & `download-center-5.3.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:45:36.877289 download-center-5.3.6/
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1537 2024-05-15 02:45:36.877171 download-center-5.3.6/PKG-INFO
--rw-r--r--   0 berry-zhang   (501) staff       (20)      888 2024-05-15 02:43:55.000000 download-center-5.3.6/README.md
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:45:36.871777 download-center-5.3.6/download_center/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/config.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:45:36.872484 download-center-5.3.6/download_center/new_spider/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/__init__.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:45:36.873216 download-center-5.3.6/download_center/new_spider/downloader/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/downloader/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/downloader/config.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     7982 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/downloader/downloader.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      254 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/downloader/html_capture.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      260 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/downloader/html_downloader.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     9176 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/downloader/html_local_downloader.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      251 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/downloader/html_render.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:45:36.873553 download-center-5.3.6/download_center/new_spider/spider/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/spider/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)    16634 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/spider/basespider.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     4675 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/spider/spider.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:45:36.875431 download-center-5.3.6/download_center/new_spider/util/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)    71351 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/ua_mobile_list.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)    47414 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/ua_pc_list.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)      471 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/ua_spider_list.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)    37353 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/util_baidu.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)    12709 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/util_baidu_relate.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      323 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/util_md5.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      540 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/util_ping.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      777 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/util_url.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      709 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/new_spider/util/util_useragent.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)       14 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/requirements.txt
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:45:36.876495 download-center-5.3.6/download_center/store/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     3147 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/baidu_cookies.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      770 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/config.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     9132 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/py_store_mysql_pool.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/store_cache.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     3285 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/store_es.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     4039 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/store_es_v2.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/store_file.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)      739 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/store_mongo.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     2014 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/store/store_oss.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:45:36.877012 download-center-5.3.6/download_center/util/
--rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/util/__init__.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     6124 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/util/py_util_basestore.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     2409 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/util/util_log.py
--rw-r--r--   0 berry-zhang   (501) staff       (20)     2480 2024-05-15 02:43:55.000000 download-center-5.3.6/download_center/util/util_log_v2.py
-drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:45:36.872388 download-center-5.3.6/download_center.egg-info/
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1537 2024-05-15 02:45:36.000000 download-center-5.3.6/download_center.egg-info/PKG-INFO
--rw-r--r--   0 berry-zhang   (501) staff       (20)     1838 2024-05-15 02:45:36.000000 download-center-5.3.6/download_center.egg-info/SOURCES.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)        1 2024-05-15 02:45:36.000000 download-center-5.3.6/download_center.egg-info/dependency_links.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)      106 2024-05-15 02:45:36.000000 download-center-5.3.6/download_center.egg-info/requires.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)       16 2024-05-15 02:45:36.000000 download-center-5.3.6/download_center.egg-info/top_level.txt
--rw-r--r--   0 berry-zhang   (501) staff       (20)       38 2024-05-15 02:45:36.877324 download-center-5.3.6/setup.cfg
--rw-r--r--   0 berry-zhang   (501) staff       (20)     4025 2024-05-15 02:43:55.000000 download-center-5.3.6/setup.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.847679 download-center-5.3.7/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1870 2024-05-16 10:00:07.847494 download-center-5.3.7/PKG-INFO
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      935 2024-05-16 10:00:03.000000 download-center-5.3.7/README.md
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.842227 download-center-5.3.7/download_center/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/config.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.842904 download-center-5.3.7/download_center/new_spider/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/__init__.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.843814 download-center-5.3.7/download_center/new_spider/downloader/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1347 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/config.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     7982 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/downloader.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      254 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/html_capture.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      260 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/html_downloader.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     9176 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/html_local_downloader.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      251 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/downloader/html_render.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.844174 download-center-5.3.7/download_center/new_spider/spider/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/spider/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    16634 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/spider/basespider.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4675 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/spider/spider.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.845536 download-center-5.3.7/download_center/new_spider/util/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    71351 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/ua_mobile_list.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    47414 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/ua_pc_list.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      471 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/ua_spider_list.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    37369 2024-05-16 09:59:13.000000 download-center-5.3.7/download_center/new_spider/util/util_baidu.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)    12709 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_baidu_relate.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      323 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_md5.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      540 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_ping.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      777 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_url.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      709 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/new_spider/util/util_useragent.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       14 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/requirements.txt
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.846807 download-center-5.3.7/download_center/store/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     3147 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/baidu_cookies.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      770 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/config.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     9132 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/py_store_mysql_pool.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_cache.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     3285 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_es.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4039 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_es_v2.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_file.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      739 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_mongo.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2014 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/store/store_oss.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.847277 download-center-5.3.7/download_center/util/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        0 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/util/__init__.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     6124 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/util/py_util_basestore.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2409 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/util/util_log.py
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     2480 2024-05-15 02:43:55.000000 download-center-5.3.7/download_center/util/util_log_v2.py
+drwxr-xr-x   0 berry-zhang   (501) staff       (20)        0 2024-05-16 10:00:07.842776 download-center-5.3.7/download_center.egg-info/
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1870 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/PKG-INFO
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     1838 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/SOURCES.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)        1 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/dependency_links.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)      106 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/requires.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       16 2024-05-16 10:00:07.000000 download-center-5.3.7/download_center.egg-info/top_level.txt
+-rw-r--r--   0 berry-zhang   (501) staff       (20)       38 2024-05-16 10:00:07.847728 download-center-5.3.7/setup.cfg
+-rw-r--r--   0 berry-zhang   (501) staff       (20)     4025 2024-05-16 10:00:03.000000 download-center-5.3.7/setup.py
```

### Comparing `download-center-5.3.6/README.md` & `download-center-5.3.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 - 5.2.16: pymysql版本写法问题
 - 5.2.18: v1.0.0及以上请使用from pymysql.converters import escape_string
 - 5.3.0: 使用私有网络 172.17.0.*
 - 5.3.1: spider里可以打印当前ip
 - 5.3.2: 登录是判断当前ip
 - 5.3.3: 添加百度工具包：pc，mb请求头 + 获取真实url
 - 5.3.5: 添加本地模式代理
+- 5.3.7: config 配置文件路径错误问题
 
 
 #### 新下载中心参数，参考 newDownloadReadme.md 文件
 
 使用方法：
 config={"param": {"et":13,'cu',url}}
 request = SpiderRequest(headers=headers, urls=urls,config = config)
```

### Comparing `download-center-5.3.6/download_center/config.py` & `download-center-5.3.7/download_center/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/downloader/config.py` & `download-center-5.3.7/download_center/new_spider/downloader/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/downloader/downloader.py` & `download-center-5.3.7/download_center/new_spider/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/downloader/html_local_downloader.py` & `download-center-5.3.7/download_center/new_spider/downloader/html_local_downloader.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/spider/basespider.py` & `download-center-5.3.7/download_center/new_spider/spider/basespider.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/spider/spider.py` & `download-center-5.3.7/download_center/new_spider/spider/spider.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/util/ua_mobile_list.txt` & `download-center-5.3.7/download_center/new_spider/util/ua_mobile_list.txt`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/util/ua_pc_list.txt` & `download-center-5.3.7/download_center/new_spider/util/ua_pc_list.txt`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/util/util_baidu.py` & `download-center-5.3.7/download_center/new_spider/util/util_baidu.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import requests
 from lxml import etree
 import redis
 import time
 
 from lxml.html import fromstring
 
-import config as pro_config
+import download_center.config as pro_config
 from download_center.store import config
 from http import cookiejar
 from urllib.request import Request, HTTPCookieProcessor, build_opener
 
 from pymysql.converters import escape_string
```

### Comparing `download-center-5.3.6/download_center/new_spider/util/util_baidu_relate.py` & `download-center-5.3.7/download_center/new_spider/util/util_baidu_relate.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/util/util_ping.py` & `download-center-5.3.7/download_center/new_spider/util/util_ping.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/util/util_url.py` & `download-center-5.3.7/download_center/new_spider/util/util_url.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/new_spider/util/util_useragent.py` & `download-center-5.3.7/download_center/new_spider/util/util_useragent.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/store/baidu_cookies.py` & `download-center-5.3.7/download_center/store/baidu_cookies.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/store/config.py` & `download-center-5.3.7/download_center/store/config.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/store/py_store_mysql_pool.py` & `download-center-5.3.7/download_center/store/py_store_mysql_pool.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/store/store_es.py` & `download-center-5.3.7/download_center/store/store_es.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/store/store_es_v2.py` & `download-center-5.3.7/download_center/store/store_es_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/store/store_mongo.py` & `download-center-5.3.7/download_center/store/store_mongo.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/store/store_oss.py` & `download-center-5.3.7/download_center/store/store_oss.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/util/py_util_basestore.py` & `download-center-5.3.7/download_center/util/py_util_basestore.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/util/util_log.py` & `download-center-5.3.7/download_center/util/util_log.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center/util/util_log_v2.py` & `download-center-5.3.7/download_center/util/util_log_v2.py`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/download_center.egg-info/SOURCES.txt` & `download-center-5.3.7/download_center.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `download-center-5.3.6/setup.py` & `download-center-5.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'download-center'
 DESCRIPTION = 'spider framework for winndoo.'
 URL = 'http://git.winndoo.cn:82/python/download_center/downloader_client.git'
 EMAIL = 'baozhu.zhang@winndoo.com'
 AUTHOR = 'Welcome#1'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '5.3.6'
+VERSION = '5.3.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'pymongo',
     'oss2',
     'redis',
     'DBUtils',
```

