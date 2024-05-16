# Comparing `tmp/tsugu-api-python-1.1.3.tar.gz` & `tmp/tsugu-api-python-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-api-python-1.1.3.tar", last modified: Wed May 15 16:09:12 2024, max compression
+gzip compressed data, was "tsugu-api-python-1.1.4.tar", last modified: Thu May 16 00:36:43 2024, max compression
```

## Comparing `tsugu-api-python-1.1.3.tar` & `tsugu-api-python-1.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:09:12.107467 tsugu-api-python-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-15 16:09:12.107467 tsugu-api-python-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:09:12.107467 tsugu-api-python-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:09:12.103467 tsugu-api-python-1.1.3/tsugu_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:09:12.103467 tsugu-api-python-1.1.3/tsugu_api_async/
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_bandoristation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_station.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_tsugu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-15 16:09:02.000000 tsugu-api-python-1.1.3/tsugu_api_async/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:09:12.107467 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-15 16:09:11.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-15 16:09:12.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:09:11.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-15 16:09:11.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 16:09:11.000000 tsugu-api-python-1.1.3/tsugu_api_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/tsugu_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/tsugu_api_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_bandoristation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_station.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_tsugu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-16 00:36:34.000000 tsugu-api-python-1.1.4/tsugu_api_async/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:36:43.002552 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 00:36:42.000000 tsugu-api-python-1.1.4/tsugu_api_python.egg-info/top_level.txt
```

### Comparing `tsugu-api-python-1.1.3/LICENSE` & `tsugu-api-python-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/PKG-INFO` & `tsugu-api-python-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.3 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.4 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.3/README.md` & `tsugu-api-python-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/setup.py` & `tsugu-api-python-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu-api-python',
-    version='1.1.3',
+    version='1.1.4',
     author='WindowsSov8',
     author_email='qwertyuiop2333@hotmail.com',
     description='Tsugu BanGDream Bot 的功能 API 统合包',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WindowsSov8forUs/tsugu-api-python',
     include_package_data=False,
```

### Comparing `tsugu-api-python-1.1.3/tsugu_api/__init__.py` & `tsugu-api-python-1.1.4/tsugu_api/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api/_bandoristation.py` & `tsugu-api-python-1.1.4/tsugu_api/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api/_network.py` & `tsugu-api-python-1.1.4/tsugu_api/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api/_station.py` & `tsugu-api-python-1.1.4/tsugu_api/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api/_tsugu.py` & `tsugu-api-python-1.1.4/tsugu_api/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api/_typing.py` & `tsugu-api-python-1.1.4/tsugu_api/_typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,16 @@
     bindingStatus: Literal[0, 1, 2]
     verifyCode: NotRequired[int]
 
 class _TsuguUser(TypedDict):
     '''用户数据'''
     user_id: str
     platform: str
-    server_mode: _Server
-    default_server: list[_Server]
+    server_mode: _ServerId
+    default_server: list[_ServerId]
     car: bool
     server_list: list[_TsuguUserServer]
 
 class _GetUserDataResponse(TypedDict):
     '''`/user/getUserData` 响应结果'''
     status: _Status
     data: Union[str, _TsuguUser]
```

### Comparing `tsugu-api-python-1.1.3/tsugu_api/_user.py` & `tsugu-api-python-1.1.4/tsugu_api/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api/settings.py` & `tsugu-api-python-1.1.4/tsugu_api/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api/utils.py` & `tsugu-api-python-1.1.4/tsugu_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api_async/__init__.py` & `tsugu-api-python-1.1.4/tsugu_api_async/__init__.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api_async/_bandoristation.py` & `tsugu-api-python-1.1.4/tsugu_api_async/_bandoristation.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api_async/_network.py` & `tsugu-api-python-1.1.4/tsugu_api_async/_network.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api_async/_station.py` & `tsugu-api-python-1.1.4/tsugu_api_async/_station.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api_async/_tsugu.py` & `tsugu-api-python-1.1.4/tsugu_api_async/_tsugu.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api_async/_typing.py` & `tsugu-api-python-1.1.4/tsugu_api_async/_typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,16 +87,16 @@
     bindingStatus: Literal[0, 1, 2]
     verifyCode: NotRequired[int]
 
 class _TsuguUser(TypedDict):
     '''用户数据'''
     user_id: str
     platform: str
-    server_mode: _Server
-    default_server: list[_Server]
+    server_mode: _ServerId
+    default_server: list[_ServerId]
     car: bool
     server_list: list[_TsuguUserServer]
 
 class _GetUserDataResponse(TypedDict):
     '''`/user/getUserData` 响应结果'''
     status: _Status
     data: Union[str, _TsuguUser]
```

### Comparing `tsugu-api-python-1.1.3/tsugu_api_async/_user.py` & `tsugu-api-python-1.1.4/tsugu_api_async/_user.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api_async/settings.py` & `tsugu-api-python-1.1.4/tsugu_api_async/settings.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api_async/utils.py` & `tsugu-api-python-1.1.4/tsugu_api_async/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-api-python-1.1.3/tsugu_api_python.egg-info/PKG-INFO` & `tsugu-api-python-1.1.4/tsugu_api_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu-api-python
-Version: 1.1.3
+Version: 1.1.4
 Summary: Tsugu BanGDream Bot 的功能 API 统合包
 Home-page: https://github.com/WindowsSov8forUs/tsugu-api-python
 Author: WindowsSov8
 Author-email: qwertyuiop2333@hotmail.com
 License: MIT
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.3 Summary: Tsugu
+Metadata-Version: 2.1 Name: tsugu-api-python Version: 1.1.4 Summary: Tsugu
 BanGDream Bot çåè½ API ç»åå Home-page: https://github.com/
 WindowsSov8forUs/tsugu-api-python Author: WindowsSov8 Author-email:
 qwertyuiop2333@hotmail.com License: MIT Description:
  ![tsugu-api-ython logo](https://github.com/WindowsSov8forUs/tsugu-api-python/
          blob/main/logo.png) # tsugu-api-python _â¨ Python ç¼åç
       [TsuguBanGDreamBot](https://github.com/Yamamoto-2/tsugu-bangdream-
          bot?tab=readme-ov-file) ç¸å³åç§åè½ API è°ç¨åº â¨_
```

### Comparing `tsugu-api-python-1.1.3/tsugu_api_python.egg-info/SOURCES.txt` & `tsugu-api-python-1.1.4/tsugu_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

