# Comparing `tmp/wipdevice-0.0.1.tar.gz` & `tmp/wipdevice-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wipdevice-0.0.1.tar", last modified: Thu May 16 08:02:38 2024, max compression
+gzip compressed data, was "dist\wipdevice-0.0.2.tar", last modified: Thu May 16 09:03:06 2024, max compression
```

## Comparing `wipdevice-0.0.1.tar` & `wipdevice-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:38.000000 wipdevice-0.0.1/
--rw-rw-rw-   0        0        0      623 2024-05-16 08:02:38.000000 wipdevice-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-16 07:58:46.000000 wipdevice-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1962 2024-05-16 07:53:50.000000 wipdevice-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 08:02:38.000000 wipdevice-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      862 2024-05-16 08:02:23.000000 wipdevice-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:38.000000 wipdevice-0.0.1/WIPClient/
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:38.000000 wipdevice-0.0.1/WIPClient/interface/
--rw-rw-rw-   0        0        0    16050 2023-06-19 03:31:42.000000 wipdevice-0.0.1/WIPClient/interface/HTTPSocketManager.py
--rw-rw-rw-   0        0        0     8506 2023-04-25 00:41:05.000000 wipdevice-0.0.1/WIPClient/interface/SocketManager.py
--rw-rw-rw-   0        0        0    21703 2024-04-24 09:34:42.000000 wipdevice-0.0.1/WIPClient/interface/SocketManagerV2.py
--rw-rw-rw-   0        0        0     3476 2023-04-25 00:41:05.000000 wipdevice-0.0.1/WIPClient/interface/WebSocketManager.py
--rw-rw-rw-   0        0        0        4 2023-04-25 00:41:05.000000 wipdevice-0.0.1/WIPClient/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:38.000000 wipdevice-0.0.1/WIPClient/protocol/
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:38.000000 wipdevice-0.0.1/WIPClient/protocol/advanced/
--rw-rw-rw-   0        0        0     1249 2024-05-10 07:10:34.000000 wipdevice-0.0.1/WIPClient/protocol/advanced/aes256.py
--rw-rw-rw-   0        0        0      570 2024-05-10 07:10:34.000000 wipdevice-0.0.1/WIPClient/protocol/advanced/commonFunction.py
--rw-rw-rw-   0        0        0     5409 2024-05-10 07:10:34.000000 wipdevice-0.0.1/WIPClient/protocol/advanced/ConstantVar.py
--rw-rw-rw-   0        0        0     2448 2024-05-10 07:10:34.000000 wipdevice-0.0.1/WIPClient/protocol/advanced/JsonDataProtocol.py
--rw-rw-rw-   0        0        0      346 2024-05-10 07:10:34.000000 wipdevice-0.0.1/WIPClient/protocol/advanced/ModelJsonData.py
--rw-rw-rw-   0        0        0        4 2023-04-25 00:41:05.000000 wipdevice-0.0.1/WIPClient/protocol/advanced/__init__.py
--rw-rw-rw-   0        0        0        4 2023-04-25 00:41:05.000000 wipdevice-0.0.1/WIPClient/protocol/__init__.py
--rw-rw-rw-   0        0        0    14012 2024-05-16 04:12:16.000000 wipdevice-0.0.1/WIPClient/WIPClient.py
--rw-rw-rw-   0        0        0     1897 2024-05-16 05:39:12.000000 wipdevice-0.0.1/WIPClient/WIPClientAbstractModel.py
--rw-rw-rw-   0        0        0    14962 2024-05-16 06:36:09.000000 wipdevice-0.0.1/WIPClient/WIPClient_advance.py
--rw-rw-rw-   0        0        0    17863 2024-05-10 07:10:34.000000 wipdevice-0.0.1/WIPClient/WIPClient_advance_original.py
--rw-rw-rw-   0        0        0     2670 2024-05-16 06:34:33.000000 wipdevice-0.0.1/WIPClient/WIPDevice.py
--rw-rw-rw-   0        0        0       21 2024-05-13 12:35:25.000000 wipdevice-0.0.1/WIPClient/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 08:02:38.000000 wipdevice-0.0.1/wipdevice.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-16 08:02:38.000000 wipdevice-0.0.1/wipdevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 08:02:38.000000 wipdevice-0.0.1/wipdevice.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      623 2024-05-16 08:02:38.000000 wipdevice-0.0.1/wipdevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-05-16 08:02:38.000000 wipdevice-0.0.1/wipdevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0      884 2024-05-16 08:02:38.000000 wipdevice-0.0.1/wipdevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2024-05-16 08:02:38.000000 wipdevice-0.0.1/wipdevice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 09:03:06.000000 wipdevice-0.0.2/
+-rw-rw-rw-   0        0        0      623 2024-05-16 09:03:06.000000 wipdevice-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-16 07:58:46.000000 wipdevice-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1979 2024-05-16 08:41:57.000000 wipdevice-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 09:03:06.000000 wipdevice-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      862 2024-05-16 09:00:21.000000 wipdevice-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:03:06.000000 wipdevice-0.0.2/WIPDevice/
+drwxrwxrwx   0        0        0        0 2024-05-16 09:03:06.000000 wipdevice-0.0.2/WIPDevice/interface/
+-rw-rw-rw-   0        0        0    16050 2023-06-19 03:31:42.000000 wipdevice-0.0.2/WIPDevice/interface/HTTPSocketManager.py
+-rw-rw-rw-   0        0        0     8506 2023-04-25 00:41:05.000000 wipdevice-0.0.2/WIPDevice/interface/SocketManager.py
+-rw-rw-rw-   0        0        0    21703 2024-04-24 09:34:42.000000 wipdevice-0.0.2/WIPDevice/interface/SocketManagerV2.py
+-rw-rw-rw-   0        0        0     3476 2023-04-25 00:41:05.000000 wipdevice-0.0.2/WIPDevice/interface/WebSocketManager.py
+-rw-rw-rw-   0        0        0        4 2023-04-25 00:41:05.000000 wipdevice-0.0.2/WIPDevice/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:03:06.000000 wipdevice-0.0.2/WIPDevice/protocol/
+drwxrwxrwx   0        0        0        0 2024-05-16 09:03:06.000000 wipdevice-0.0.2/WIPDevice/protocol/advanced/
+-rw-rw-rw-   0        0        0     1249 2024-05-10 07:10:34.000000 wipdevice-0.0.2/WIPDevice/protocol/advanced/aes256.py
+-rw-rw-rw-   0        0        0      570 2024-05-10 07:10:34.000000 wipdevice-0.0.2/WIPDevice/protocol/advanced/commonFunction.py
+-rw-rw-rw-   0        0        0     5409 2024-05-10 07:10:34.000000 wipdevice-0.0.2/WIPDevice/protocol/advanced/ConstantVar.py
+-rw-rw-rw-   0        0        0     2448 2024-05-10 07:10:34.000000 wipdevice-0.0.2/WIPDevice/protocol/advanced/JsonDataProtocol.py
+-rw-rw-rw-   0        0        0      346 2024-05-10 07:10:34.000000 wipdevice-0.0.2/WIPDevice/protocol/advanced/ModelJsonData.py
+-rw-rw-rw-   0        0        0        4 2023-04-25 00:41:05.000000 wipdevice-0.0.2/WIPDevice/protocol/advanced/__init__.py
+-rw-rw-rw-   0        0        0        4 2023-04-25 00:41:05.000000 wipdevice-0.0.2/WIPDevice/protocol/__init__.py
+-rw-rw-rw-   0        0        0    14012 2024-05-16 04:12:16.000000 wipdevice-0.0.2/WIPDevice/WIPClient.py
+-rw-rw-rw-   0        0        0     1897 2024-05-16 05:39:12.000000 wipdevice-0.0.2/WIPDevice/WIPClientAbstractModel.py
+-rw-rw-rw-   0        0        0    14962 2024-05-16 06:36:09.000000 wipdevice-0.0.2/WIPDevice/WIPClient_advance.py
+-rw-rw-rw-   0        0        0     2670 2024-05-16 06:34:33.000000 wipdevice-0.0.2/WIPDevice/WIPDevice.py
+-rw-rw-rw-   0        0        0       21 2024-05-16 09:01:01.000000 wipdevice-0.0.2/WIPDevice/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:03:06.000000 wipdevice-0.0.2/wipdevice.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:03:06.000000 wipdevice-0.0.2/wipdevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 08:02:38.000000 wipdevice-0.0.2/wipdevice.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      623 2024-05-16 09:03:06.000000 wipdevice-0.0.2/wipdevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-05-16 09:03:06.000000 wipdevice-0.0.2/wipdevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      844 2024-05-16 09:03:06.000000 wipdevice-0.0.2/wipdevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 09:03:06.000000 wipdevice-0.0.2/wipdevice.egg-info/top_level.txt
```

### Comparing `wipdevice-0.0.1/PKG-INFO` & `wipdevice-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipdevice
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wow IoT Platform API libraries
 Home-page: https://github.com/WOWSYSTEM/WIP-Python
 Author: wowsystem, nobu
 Author-email: contact@wowsystem.co.kr
 License: UNKNOWN
 Keywords: wowsystem,IoT,WIP,IoT Platform,IoT Server,wowsystem,WOW IoT Platform
 Platform: UNKNOWN
```

### Comparing `wipdevice-0.0.1/README.md` & `wipdevice-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 WOW IoT Platform과 연동하여 사용할 수 있는 Python 라이브러리이다.
 간편하게 IoT Platform과 연동하여, 데이터 전송 및 제어 명령 수신이 가능하다.
 
 디바이스를 연동하기 위해선 IoT Platform에 로그인 후 디바이스를 등록하여야 사용할 수 있다.
 
 해당 라이브러리 개발 시 다양한 테스트 조건에도 문제 없이 Platform에 접속하여 사용할 수 있도록 최선을 다한다.
 
-
 ## Getting Started
 - Python3.6 버전 이상 파이썬 설치
 - Visual Code 등으로 수정 가능
 - 최종 및 안정화 버전은 PyPI에 업로드 할 수 있으며, 관련 방법은 사내에서 공유되는 자료를 확인
 
 
 ### Installing
@@ -32,17 +31,19 @@
 pip install Crypto
 ```
 
 ### Versioning
 * 업데이트 시 반드시 버전 관련 설정 수정할 것
 * 버전 수정안할 시 업데이트 사항이 정상적으로 적용안될 수 있다.
 
+## PyPI
+(https://pypi.org/project/wipdevice/)
 
 ## Built With / 누구랑 만들었나요?
-* [이승명(nobu)](nobu1015@naver.com, nobu1015@wowsystem.co.kr) - 무엇 무엇을 했어요
+* [이승명(nobu)](nobu1015@naver.com, nobu1015@wowsystem.co.kr)
 
 ## Contributiong / 기여
 
 Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us. / [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) 를 읽고 이에 맞추어 pull request 를 해주세요.
 
 ## License / 라이센스
 협의 필요
```

### Comparing `wipdevice-0.0.1/setup.py` & `wipdevice-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wipdevice',
-    version='0.0.1', # 수정되면 꼭 version 업데이트하기
+    version='0.0.2', # 수정되면 꼭 version 업데이트하기
     description='Wow IoT Platform API libraries',
     author='wowsystem, nobu',
     author_email='contact@wowsystem.co.kr',
     url='https://github.com/WOWSYSTEM/WIP-Python',
     install_requires=['Crypto', ],
     packages=find_packages(exclude=[]),
     keywords=['wowsystem', 'IoT', 'WIP', 'IoT Platform', 'IoT Server', 'wowsystem', 'WOW IoT Platform'],
```

### Comparing `wipdevice-0.0.1/WIPClient/interface/HTTPSocketManager.py` & `wipdevice-0.0.2/WIPDevice/interface/HTTPSocketManager.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/interface/SocketManager.py` & `wipdevice-0.0.2/WIPDevice/interface/SocketManager.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/interface/SocketManagerV2.py` & `wipdevice-0.0.2/WIPDevice/interface/SocketManagerV2.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/interface/WebSocketManager.py` & `wipdevice-0.0.2/WIPDevice/interface/WebSocketManager.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/protocol/advanced/aes256.py` & `wipdevice-0.0.2/WIPDevice/protocol/advanced/aes256.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/protocol/advanced/commonFunction.py` & `wipdevice-0.0.2/WIPDevice/protocol/advanced/commonFunction.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/protocol/advanced/ConstantVar.py` & `wipdevice-0.0.2/WIPDevice/protocol/advanced/ConstantVar.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/protocol/advanced/JsonDataProtocol.py` & `wipdevice-0.0.2/WIPDevice/protocol/advanced/JsonDataProtocol.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/WIPClient.py` & `wipdevice-0.0.2/WIPDevice/WIPClient.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/WIPClientAbstractModel.py` & `wipdevice-0.0.2/WIPDevice/WIPClientAbstractModel.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/WIPClient_advance.py` & `wipdevice-0.0.2/WIPDevice/WIPClient_advance.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/WIPClient/WIPDevice.py` & `wipdevice-0.0.2/WIPDevice/WIPDevice.py`

 * *Files identical despite different names*

### Comparing `wipdevice-0.0.1/wipdevice.egg-info/PKG-INFO` & `wipdevice-0.0.2/wipdevice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipdevice
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wow IoT Platform API libraries
 Home-page: https://github.com/WOWSYSTEM/WIP-Python
 Author: wowsystem, nobu
 Author-email: contact@wowsystem.co.kr
 License: UNKNOWN
 Keywords: wowsystem,IoT,WIP,IoT Platform,IoT Server,wowsystem,WOW IoT Platform
 Platform: UNKNOWN
```

