# Comparing `tmp/jeedomdaemon-0.9.5.tar.gz` & `tmp/jeedomdaemon-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.9.5.tar", last modified: Mon May 13 09:13:29 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.9.6.tar", last modified: Thu May 16 16:21:35 2024, max compression
```

## Comparing `jeedomdaemon-0.9.5.tar` & `jeedomdaemon-0.9.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:35.248139 jeedomdaemon-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-16 16:21:35.248139 jeedomdaemon-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:35.244139 jeedomdaemon-0.9.6/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:35.248139 jeedomdaemon-0.9.6/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-16 16:21:35.000000 jeedomdaemon-0.9.6/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-16 16:21:35.000000 jeedomdaemon-0.9.6/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:21:35.000000 jeedomdaemon-0.9.6/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 16:21:35.000000 jeedomdaemon-0.9.6/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 16:21:35.000000 jeedomdaemon-0.9.6/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:21:35.248139 jeedomdaemon-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:35.248139 jeedomdaemon-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-16 16:21:30.000000 jeedomdaemon-0.9.6/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.9.5/LICENSE` & `jeedomdaemon-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.5/PKG-INFO` & `jeedomdaemon-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.9.5
+Version: 0.9.6
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Keywords: JEEDOM,DAEMON,ASYNCIO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jeedomdaemon-0.9.5/README.md` & `jeedomdaemon-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.5/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.9.6/jeedomdaemon/aio_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                     return False
         except aiohttp.ClientError as e:
             self._logger.error('Callback error: %s. Please check your network configuration page', e)
             return False
         return True
 
     async def __send_task(self):
-        self._logger.info("Send async started")
+        self._logger.info("Send async started with a cycle of %ss", self._cycle)
         try:
             last_send_on_error = False
             while True:
                 if len(self.__changes)>0:
                     changes = self.__changes
                     self.__changes = {}
```

### Comparing `jeedomdaemon-0.9.5/jeedomdaemon/base_config.py` & `jeedomdaemon-0.9.6/jeedomdaemon/base_config.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.5/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.9.6/jeedomdaemon/base_daemon.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.5/jeedomdaemon/utils.py` & `jeedomdaemon-0.9.6/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.5/jeedomdaemon.egg-info/PKG-INFO` & `jeedomdaemon-0.9.6/jeedomdaemon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.9.5
+Version: 0.9.6
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Keywords: JEEDOM,DAEMON,ASYNCIO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jeedomdaemon-0.9.5/setup.py` & `jeedomdaemon-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylint: disable=missing-module-docstring
 
 from setuptools import setup, find_packages
 
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 
 setup(
     # Needed to silence warnings (and to be a worthwhile package)
     name='jeedomdaemon',
     url='https://github.com/Mips2648/jeedom-daemon-py',
     author='Mips',
     # author_email='',
```

### Comparing `jeedomdaemon-0.9.5/tests/base_config_test.py` & `jeedomdaemon-0.9.6/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.5/tests/base_daemon_test.py` & `jeedomdaemon-0.9.6/tests/base_daemon_test.py`

 * *Files identical despite different names*

