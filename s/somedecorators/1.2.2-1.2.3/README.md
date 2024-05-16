# Comparing `tmp/somedecorators-1.2.2.tar.gz` & `tmp/somedecorators-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somedecorators-1.2.2.tar", last modified: Fri May 10 00:30:06 2024, max compression
+gzip compressed data, was "somedecorators-1.2.3.tar", last modified: Thu May 16 02:01:47 2024, max compression
```

## Comparing `somedecorators-1.2.2.tar` & `somedecorators-1.2.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-10 00:30:06.377607 somedecorators-1.2.2/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1108 2023-11-17 06:58:43.000000 somedecorators-1.2.2/LICENSE
--rw-r--r--   0 aaron     (1000) aaron     (1000)     6901 2024-05-10 00:30:06.373607 somedecorators-1.2.2/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     6100 2024-05-09 06:24:27.000000 somedecorators-1.2.2/README.md
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2024-05-10 00:30:06.377607 somedecorators-1.2.2/setup.cfg
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1959 2024-05-10 00:29:49.000000 somedecorators-1.2.2/setup.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-10 00:30:06.373607 somedecorators-1.2.2/somedecorators/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      181 2024-05-09 06:21:29.000000 somedecorators-1.2.2/somedecorators/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-10 00:30:06.373607 somedecorators-1.2.2/somedecorators/conf/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     8478 2023-12-13 06:34:22.000000 somedecorators-1.2.2/somedecorators/conf/__init__.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    21956 2023-12-13 06:17:27.000000 somedecorators-1.2.2/somedecorators/conf/global_settings.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2330 2023-12-13 06:20:12.000000 somedecorators-1.2.2/somedecorators/email.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1903 2024-05-10 00:24:21.000000 somedecorators-1.2.2/somedecorators/log.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2056 2023-11-17 06:58:43.000000 somedecorators-1.2.2/somedecorators/retry.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1331 2023-11-17 06:58:43.000000 somedecorators-1.2.2/somedecorators/timeit.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2786 2023-12-13 06:55:17.000000 somedecorators-1.2.2/somedecorators/wechat.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-10 00:30:06.373607 somedecorators-1.2.2/somedecorators.egg-info/
--rw-r--r--   0 aaron     (1000) aaron     (1000)     6901 2024-05-10 00:30:06.000000 somedecorators-1.2.2/somedecorators.egg-info/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      466 2024-05-10 00:30:06.000000 somedecorators-1.2.2/somedecorators.egg-info/SOURCES.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2024-05-10 00:30:06.000000 somedecorators-1.2.2/somedecorators.egg-info/dependency_links.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       43 2024-05-10 00:30:06.000000 somedecorators-1.2.2/somedecorators.egg-info/requires.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       15 2024-05-10 00:30:06.000000 somedecorators-1.2.2/somedecorators.egg-info/top_level.txt
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-10 00:30:06.373607 somedecorators-1.2.2/tests/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      316 2024-05-10 00:28:09.000000 somedecorators-1.2.2/tests/test_log.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1902 2023-12-13 06:42:25.000000 somedecorators-1.2.2/tests/tests.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-16 02:01:47.830123 somedecorators-1.2.3/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1108 2023-11-17 06:58:43.000000 somedecorators-1.2.3/LICENSE
+-rw-r--r--   0 aaron     (1000) aaron     (1000)     7657 2024-05-16 02:01:47.830123 somedecorators-1.2.3/PKG-INFO
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     6827 2024-05-16 02:00:20.000000 somedecorators-1.2.3/README.md
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2024-05-16 02:01:47.830123 somedecorators-1.2.3/setup.cfg
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1985 2024-05-16 01:43:06.000000 somedecorators-1.2.3/setup.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-16 02:01:47.826123 somedecorators-1.2.3/somedecorators/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      215 2024-05-16 01:58:18.000000 somedecorators-1.2.3/somedecorators/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-16 02:01:47.830123 somedecorators-1.2.3/somedecorators/conf/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     8478 2023-12-13 06:34:22.000000 somedecorators-1.2.3/somedecorators/conf/__init__.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    21956 2023-12-13 06:17:27.000000 somedecorators-1.2.3/somedecorators/conf/global_settings.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1512 2024-05-16 01:40:59.000000 somedecorators-1.2.3/somedecorators/config.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2330 2023-12-13 06:20:12.000000 somedecorators-1.2.3/somedecorators/email.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2012 2024-05-16 01:40:49.000000 somedecorators-1.2.3/somedecorators/log.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2056 2023-11-17 06:58:43.000000 somedecorators-1.2.3/somedecorators/retry.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1331 2023-11-17 06:58:43.000000 somedecorators-1.2.3/somedecorators/timeit.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2786 2023-12-13 06:55:17.000000 somedecorators-1.2.3/somedecorators/wechat.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-16 02:01:47.830123 somedecorators-1.2.3/somedecorators.egg-info/
+-rw-r--r--   0 aaron     (1000) aaron     (1000)     7657 2024-05-16 02:01:47.000000 somedecorators-1.2.3/somedecorators.egg-info/PKG-INFO
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      491 2024-05-16 02:01:47.000000 somedecorators-1.2.3/somedecorators.egg-info/SOURCES.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2024-05-16 02:01:47.000000 somedecorators-1.2.3/somedecorators.egg-info/dependency_links.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       57 2024-05-16 02:01:47.000000 somedecorators-1.2.3/somedecorators.egg-info/requires.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       15 2024-05-16 02:01:47.000000 somedecorators-1.2.3/somedecorators.egg-info/top_level.txt
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-16 02:01:47.830123 somedecorators-1.2.3/tests/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      316 2024-05-10 00:28:09.000000 somedecorators-1.2.3/tests/test_log.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1902 2023-12-13 06:42:25.000000 somedecorators-1.2.3/tests/tests.py
```

### Comparing `somedecorators-1.2.2/LICENSE` & `somedecorators-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2.2/PKG-INFO` & `somedecorators-1.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,19 @@
-Metadata-Version: 2.1
-Name: somedecorators
-Version: 1.2.2
-Summary: Some useful decorators in Python.
-Home-page: https://github.com/somenzz/somedecorators
-Author: somenzz
-Author-email: somenzz@163.com
-License: MIT
-Keywords: awesome decorators
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: djangomail==0.8
-Requires-Dist: wechat-enterprise-sdk==0.4
-
 # somedecorators
 
-some very useful decorators for python 
+Some very useful Python decorators, functions, classes, continuously updated.
+
+
+一些非常实用的 Python 装饰器、函数、类，持续更新。
 
-一些非常实用的 Python 装饰器，持续更新
+- 新增 wechat_on_exception，报错发送企业微信 :  from somedecorators import wechat_on_exception
+- 新增 setup_logger，快速配置日志  : from somedecorators import setup_logger  
+- 新增 ConfigManager，快速搞定配置文件 : from somedecorators import ConfigManager 
 
-- 新增 wechat_on_exception  from somedecorators import wechat_on_exception
+使用方法如下：
 
 ## 安装
 
 ```sh
 pip install somedecorators
 ```
 
@@ -253,23 +235,36 @@
     elif args == 2:
         raise Exception2
     else:
         raise Exception3
 ```
 
 
-#### setup_logger
+#### 快速配置日志 setup_logger
 
 一个简单的使用日志的方法
 
 ```python
 from somedecorators import setup_logger
 logger = setup_logger("myapp")
 logger.info("hello this is myapp log")
+logger2 = setup_logger("myapp2", log_path="./log/app.log")
+logger3 = setup_logger("myapp3",handlers=['console']) 
+logger4 = setup_logger("myapp4",handlers=['console','file']) 
 ```
 
+#### 快速搞定配置文件
+
+```python
+from somedecorators import ConfigManager
+config_manager = ConfigManager("config.yml")
+config_data = config_manager.get_all()
+print(config_data)
+```
 
 ## 参与项目
 
-欢迎分享你最常用的装饰器，加入到这里。
+欢迎分享你最常用的装饰器、类、函数，加入到这里。
 
+## 联系我 
 
+微信：somenzz-enjoy
```

### Comparing `somedecorators-1.2.2/README.md` & `somedecorators-1.2.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,43 @@
+Metadata-Version: 2.1
+Name: somedecorators
+Version: 1.2.3
+Summary: Some useful decorators in Python.
+Home-page: https://github.com/somenzz/somedecorators
+Author: somenzz
+Author-email: somenzz@163.com
+License: MIT
+Keywords: awesome decorators
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: djangomail==0.8
+Requires-Dist: wechat-enterprise-sdk==0.4
+Requires-Dist: PyYAML==6.0.1
+
 # somedecorators
 
-some very useful decorators for python 
+Some very useful Python decorators, functions, classes, continuously updated.
+
+
+一些非常实用的 Python 装饰器、函数、类，持续更新。
 
-一些非常实用的 Python 装饰器，持续更新
+- 新增 wechat_on_exception，报错发送企业微信 :  from somedecorators import wechat_on_exception
+- 新增 setup_logger，快速配置日志  : from somedecorators import setup_logger  
+- 新增 ConfigManager，快速搞定配置文件 : from somedecorators import ConfigManager 
 
-- 新增 wechat_on_exception  from somedecorators import wechat_on_exception
+使用方法如下：
 
 ## 安装
 
 ```sh
 pip install somedecorators
 ```
 
@@ -230,23 +259,36 @@
     elif args == 2:
         raise Exception2
     else:
         raise Exception3
 ```
 
 
-#### setup_logger
+#### 快速配置日志 setup_logger
 
 一个简单的使用日志的方法
 
 ```python
 from somedecorators import setup_logger
 logger = setup_logger("myapp")
 logger.info("hello this is myapp log")
+logger2 = setup_logger("myapp2", log_path="./log/app.log")
+logger3 = setup_logger("myapp3",handlers=['console']) 
+logger4 = setup_logger("myapp4",handlers=['console','file']) 
 ```
 
+#### 快速搞定配置文件
+
+```python
+from somedecorators import ConfigManager
+config_manager = ConfigManager("config.yml")
+config_data = config_manager.get_all()
+print(config_data)
+```
 
 ## 参与项目
 
-欢迎分享你最常用的装饰器，加入到这里。
+欢迎分享你最常用的装饰器、类、函数，加入到这里。
 
+## 联系我 
 
+微信：somenzz-enjoy
```

### Comparing `somedecorators-1.2.2/setup.py` & `somedecorators-1.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 readme = Path("README.md")
 license = Path("LICENSE")
 
 
 # Read the version without importing the package
 # (and thus attempting to import packages it depends on that may not be
 # installed yet)
-version = "1.2.2"
+version = "1.2.3"
 
 NAME = 'somedecorators'
 VERSION = version
 DESCRIPTION = 'Some useful decorators in Python.'
 KEYWORDS = 'awesome decorators'
 AUTHOR = 'somenzz'
 AUTHOR_EMAIL = 'somenzz@163.com'
 URL = 'https://github.com/somenzz/somedecorators'
 LICENSE = license.read_text()
 PACKAGES = find_packages(exclude=['tests', 'tests.*'])
 
 INSTALL_REQUIRES = [
          'djangomail==0.8', 
-         'wechat-enterprise-sdk==0.4'
+         'wechat-enterprise-sdk==0.4',
+         'PyYAML==6.0.1'
       ]
 TEST_SUITE = 'tests'
 TESTS_REQUIRE = []
 
 CLASSIFIERS = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `somedecorators-1.2.2/somedecorators/conf/__init__.py` & `somedecorators-1.2.3/somedecorators/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2.2/somedecorators/conf/global_settings.py` & `somedecorators-1.2.3/somedecorators/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2.2/somedecorators/email.py` & `somedecorators-1.2.3/somedecorators/email.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2.2/somedecorators/log.py` & `somedecorators-1.2.3/somedecorators/log.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,57 @@
-import logging.config
-import os
-import sys
-
-
-def setup_logger(name=""):
-    os.makedirs("logs", exist_ok=True)
-    LOGGING_CONFIG = {
-        "version": 1,
-        "disable_existing_loggers": False,
-        "formatters": {
-            "detailed": {
-                "format": "%(asctime)s [%(process)d] [%(thread)d] [%(levelname)s] [%(module)s:%(lineno)d] - %(message)s"
-            },
-            "simple": {
-                "format": "%(asctime)s - %(levelname)s [%(module)s:%(lineno)d] - %(message)s"
-            },
-        },
-        "handlers": {
-            "console": {
-                "class": "logging.StreamHandler",
-                "level": "DEBUG",
-                "formatter": "simple",
-                "stream": "ext://sys.stdout",
-            },
-            "file": {
-                "class": "logging.handlers.RotatingFileHandler",
-                "level": "INFO",
-                "formatter": "detailed",
-                "filename": "logs/application.log",
-                "maxBytes": 10485760,  # 10MB
-                "backupCount": 5,
-                "encoding": "utf8",
-            },
-        },
-        "loggers": {
-            "": {  # root logger
-                "handlers": ["console", "file"],
-                "level": "DEBUG",
-                "propagate": True,
-            }
-        },
-    }
-
-    logging.config.dictConfig(LOGGING_CONFIG)
-    return logging.getLogger(name)
-
-
-def handle_exception(exc_type, exc_value, exc_traceback):
-    """Log any uncaught exceptions."""
-    if issubclass(exc_type, KeyboardInterrupt):
-        # Do not log or print KeyboardInterrupt exceptions (like Ctrl+C)
-        sys.__excepthook__(exc_type, exc_value, exc_traceback)
-        return
-    logger = setup_logger()
-    logger.error("Uncaught exception", exc_info=(exc_type, exc_value, exc_traceback))
-
-
-# Set the global exception hook to our custom function
-sys.excepthook = handle_exception
+import logging.config
+import os
+import sys
+
+def setup_logger(name="", log_path="logs/application.log", handlers=["console", "file"]):
+    os.makedirs(os.path.dirname(log_path), exist_ok=True)
+    LOGGING_CONFIG = {
+        "version": 1,
+        "disable_existing_loggers": False,
+        "formatters": {
+            "detailed": {
+                "format": "%(asctime)s [%(process)d] [%(thread)d] [%(levelname)s] [%(module)s:%(lineno)d] - %(message)s"
+            },
+            "simple": {
+                "format": "%(asctime)s - %(levelname)s [%(module)s:%(lineno)d] - %(message)s"
+            },
+        },
+        "handlers": {
+            "console": {
+                "class": "logging.StreamHandler",
+                "level": "DEBUG",
+                "formatter": "simple",
+                "stream": "ext://sys.stdout",
+            },
+            "file": {
+                "class": "logging.handlers.RotatingFileHandler",
+                "level": "INFO",
+                "formatter": "detailed",
+                "filename": log_path,
+                "maxBytes": 10485760,  # 10MB
+                "backupCount": 5,
+                "encoding": "utf8",
+            },
+        },
+        "loggers": {
+            "": {  # root logger
+                "handlers": handlers,
+                "level": "DEBUG",
+                "propagate": True,
+            }
+        },
+    }
+
+    logging.config.dictConfig(LOGGING_CONFIG)
+    return logging.getLogger(name)
+
+def handle_exception(exc_type, exc_value, exc_traceback):
+    """Log any uncaught exceptions."""
+    if issubclass(exc_type, KeyboardInterrupt):
+        # Do not log or print KeyboardInterrupt exceptions (like Ctrl+C)
+        sys.__excepthook__(exc_type, exc_value, exc_traceback)
+        return
+    logger = setup_logger()
+    logger.error("Uncaught exception", exc_info=(exc_type, exc_value, exc_traceback))
+
+# Set the global exception hook to our custom function
+sys.excepthook = handle_exception
```

### Comparing `somedecorators-1.2.2/somedecorators/retry.py` & `somedecorators-1.2.3/somedecorators/retry.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2.2/somedecorators/timeit.py` & `somedecorators-1.2.3/somedecorators/timeit.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2.2/somedecorators/wechat.py` & `somedecorators-1.2.3/somedecorators/wechat.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2.2/somedecorators.egg-info/PKG-INFO` & `somedecorators-1.2.3/somedecorators.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somedecorators
-Version: 1.2.2
+Version: 1.2.3
 Summary: Some useful decorators in Python.
 Home-page: https://github.com/somenzz/somedecorators
 Author: somenzz
 Author-email: somenzz@163.com
 License: MIT
 Keywords: awesome decorators
 Classifier: Development Status :: 3 - Alpha
@@ -16,22 +16,28 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: djangomail==0.8
 Requires-Dist: wechat-enterprise-sdk==0.4
+Requires-Dist: PyYAML==6.0.1
 
 # somedecorators
 
-some very useful decorators for python 
+Some very useful Python decorators, functions, classes, continuously updated.
 
-一些非常实用的 Python 装饰器，持续更新
 
-- 新增 wechat_on_exception  from somedecorators import wechat_on_exception
+一些非常实用的 Python 装饰器、函数、类，持续更新。
+
+- 新增 wechat_on_exception，报错发送企业微信 :  from somedecorators import wechat_on_exception
+- 新增 setup_logger，快速配置日志  : from somedecorators import setup_logger  
+- 新增 ConfigManager，快速搞定配置文件 : from somedecorators import ConfigManager 
+
+使用方法如下：
 
 ## 安装
 
 ```sh
 pip install somedecorators
 ```
 
@@ -253,23 +259,36 @@
     elif args == 2:
         raise Exception2
     else:
         raise Exception3
 ```
 
 
-#### setup_logger
+#### 快速配置日志 setup_logger
 
 一个简单的使用日志的方法
 
 ```python
 from somedecorators import setup_logger
 logger = setup_logger("myapp")
 logger.info("hello this is myapp log")
+logger2 = setup_logger("myapp2", log_path="./log/app.log")
+logger3 = setup_logger("myapp3",handlers=['console']) 
+logger4 = setup_logger("myapp4",handlers=['console','file']) 
 ```
 
+#### 快速搞定配置文件
+
+```python
+from somedecorators import ConfigManager
+config_manager = ConfigManager("config.yml")
+config_data = config_manager.get_all()
+print(config_data)
+```
 
 ## 参与项目
 
-欢迎分享你最常用的装饰器，加入到这里。
+欢迎分享你最常用的装饰器、类、函数，加入到这里。
 
+## 联系我 
 
+微信：somenzz-enjoy
```

### Comparing `somedecorators-1.2.2/tests/tests.py` & `somedecorators-1.2.3/tests/tests.py`

 * *Files identical despite different names*

