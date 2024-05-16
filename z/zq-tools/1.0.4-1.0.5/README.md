# Comparing `tmp/zq-tools-1.0.4.tar.gz` & `tmp/zq-tools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zq-tools-1.0.4.tar", last modified: Wed Apr 17 02:50:12 2024, max compression
+gzip compressed data, was "zq-tools-1.0.5.tar", last modified: Tue Apr 23 14:54:53 2024, max compression
```

## Comparing `zq-tools-1.0.4.tar` & `zq-tools-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-17 02:50:12.515524 zq-tools-1.0.4/
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     3132 2024-04-17 02:50:12.515524 zq-tools-1.0.4/PKG-INFO
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     2799 2024-04-17 02:49:29.000000 zq-tools-1.0.4/README.md
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       38 2024-04-17 02:50:12.515524 zq-tools-1.0.4/setup.cfg
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      622 2024-04-17 02:49:35.000000 zq-tools-1.0.4/setup.py
-drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-17 02:50:12.515524 zq-tools-1.0.4/test/
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       91 2022-11-19 05:19:08.000000 zq-tools-1.0.4/test/test_zq_logger.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     1051 2022-09-25 08:06:36.000000 zq-tools-1.0.4/test/test_zq_tracing.py
-drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-17 02:50:12.515524 zq-tools-1.0.4/zq_tools/
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      187 2022-11-19 05:17:23.000000 zq-tools-1.0.4/zq_tools/__init__.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      830 2022-12-21 11:09:55.000000 zq-tools-1.0.4/zq_tools/zq_cycle.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     4596 2022-10-25 03:53:08.000000 zq-tools-1.0.4/zq_tools/zq_decorator.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      520 2022-09-25 08:26:17.000000 zq-tools-1.0.4/zq_tools/zq_files.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     9435 2024-04-17 02:49:12.000000 zq-tools-1.0.4/zq_tools/zq_logger.py
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     5227 2022-10-20 06:14:14.000000 zq-tools-1.0.4/zq_tools/zq_tracing.py
-drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-17 02:50:12.515524 zq-tools-1.0.4/zq_tools.egg-info/
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     3132 2024-04-17 02:50:12.000000 zq-tools-1.0.4/zq_tools.egg-info/PKG-INFO
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      357 2024-04-17 02:50:12.000000 zq-tools-1.0.4/zq_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)        1 2024-04-17 02:50:12.000000 zq-tools-1.0.4/zq_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       23 2024-04-17 02:50:12.000000 zq-tools-1.0.4/zq_tools.egg-info/requires.txt
--rw-rw-r--   0 qzhou     (1003) qzhou     (1003)        9 2024-04-17 02:50:12.000000 zq-tools-1.0.4/zq_tools.egg-info/top_level.txt
+drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-23 14:54:53.071879 zq-tools-1.0.5/
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     3187 2024-04-23 14:54:53.071879 zq-tools-1.0.5/PKG-INFO
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     2854 2024-04-23 14:53:08.000000 zq-tools-1.0.5/README.md
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       38 2024-04-23 14:54:53.071879 zq-tools-1.0.5/setup.cfg
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      622 2024-04-23 14:51:25.000000 zq-tools-1.0.5/setup.py
+drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-23 14:54:53.071879 zq-tools-1.0.5/test/
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       91 2024-04-23 14:01:52.000000 zq-tools-1.0.5/test/test_zq_logger.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     1051 2022-09-25 08:06:36.000000 zq-tools-1.0.5/test/test_zq_tracing.py
+drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-23 14:54:53.071879 zq-tools-1.0.5/zq_tools/
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      187 2022-11-19 05:17:23.000000 zq-tools-1.0.5/zq_tools/__init__.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      830 2022-12-21 11:09:55.000000 zq-tools-1.0.5/zq_tools/zq_cycle.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     4608 2024-04-23 14:46:20.000000 zq-tools-1.0.5/zq_tools/zq_decorator.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      520 2022-09-25 08:26:17.000000 zq-tools-1.0.5/zq_tools/zq_files.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     9453 2024-04-23 14:51:10.000000 zq-tools-1.0.5/zq_tools/zq_logger.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     5227 2022-10-20 06:14:14.000000 zq-tools-1.0.5/zq_tools/zq_tracing.py
+drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-23 14:54:53.071879 zq-tools-1.0.5/zq_tools.egg-info/
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     3187 2024-04-23 14:54:52.000000 zq-tools-1.0.5/zq_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      357 2024-04-23 14:54:53.000000 zq-tools-1.0.5/zq_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)        1 2024-04-23 14:54:52.000000 zq-tools-1.0.5/zq_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       23 2024-04-23 14:54:52.000000 zq-tools-1.0.5/zq_tools.egg-info/requires.txt
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)        9 2024-04-23 14:54:52.000000 zq-tools-1.0.5/zq_tools.egg-info/top_level.txt
```

### Comparing `zq-tools-1.0.4/PKG-INFO` & `zq-tools-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of tools for zzqq2199
 Author: zzqq2199
 Author-email: zhouquanjs@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -19,14 +19,15 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
+- 1.0.5: fix bugs of `**kwargs` passing in `zq_logger`
 - 1.0.4: fix errors in logger.debug 
 - 1.0.3: make logger.debug to print without any color.
 - 1.0.2: fine grained control of different handlers
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
```

### Comparing `zq-tools-1.0.4/README.md` & `zq-tools-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
+- 1.0.5: fix bugs of `**kwargs` passing in `zq_logger`
 - 1.0.4: fix errors in logger.debug 
 - 1.0.3: make logger.debug to print without any color.
 - 1.0.2: fine grained control of different handlers
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
```

### Comparing `zq-tools-1.0.4/setup.py` & `zq-tools-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="zq-tools",
-    version="1.0.4",
+    version="1.0.5",
     author="zzqq2199",
     author_email="zhouquanjs@qq.com",
     description="A collection of tools for zzqq2199",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["zq_tools"],
     classifiers=[
```

### Comparing `zq-tools-1.0.4/test/test_zq_tracing.py` & `zq-tools-1.0.5/test/test_zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.4/zq_tools/zq_cycle.py` & `zq-tools-1.0.5/zq_tools/zq_cycle.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.4/zq_tools/zq_decorator.py` & `zq-tools-1.0.5/zq_tools/zq_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,12 +117,12 @@
         print("hello in decorator")
     test()
     
     with time_it(keyword="time it as context manager"):
         print("hello in `with`")
 
     from zq_tools.zq_logger import default_logger as logger
-    with time_it(keyword="time it as context manager", print_it=logger.info):
+    with time_it(keyword="time it as context manager", print_it=lambda x:logger.info(x)):
         print("hello in `with`, print with logger")
```

### Comparing `zq-tools-1.0.4/zq_tools/zq_files.py` & `zq-tools-1.0.5/zq_tools/zq_files.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.4/zq_tools/zq_logger.py` & `zq-tools-1.0.5/zq_tools/zq_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,23 +98,23 @@
         self._log(self.PRANK, color(msg), args, **kwargs)
     # def debug(self, msg:str, color:str='',*args, **kwargs):
     #     '''print with rank. If color is not specified, use the color format corresponding to the rank'''
     #     if not self.isEnabledFor(self.DEBUG): return
     #     color = getattr(cf, color) if color else self.default_color
     #     self._log(self.DEBUG, color(msg), args, **kwargs)
     def debug(self, msg:str, *args, **kwargs):
-        if self.isEnabledFor(logging.INFO): self._log(logging.DEBUG, msg, args, kwargs)
+        if self.isEnabledFor(logging.INFO): self._log(logging.DEBUG, msg, args, **kwargs)
     def info(self, msg:str, *args, **kwargs):
-        if self.isEnabledFor(logging.INFO): self._log(logging.INFO, cf.green(msg), args, kwargs)
+        if self.isEnabledFor(logging.INFO): self._log(logging.INFO, cf.green(msg), args, **kwargs)
     def warn(self, msg:str, *args, **kwargs):
-        if self.isEnabledFor(logging.WARN): self._log(logging.WARN, cf.yellow(msg), args, kwargs)
+        if self.isEnabledFor(logging.WARN): self._log(logging.WARN, cf.yellow(msg), args, **kwargs)
     def error(self, msg:str, *args, **kwargs):
-        if self.isEnabledFor(logging.ERROR): self._log(logging.ERROR, cf.red(msg), args, kwargs)
+        if self.isEnabledFor(logging.ERROR): self._log(logging.ERROR, cf.red(msg), args, **kwargs)
     def fatal(self, msg:str, *args, **kwargs):
-        if self.isEnabledFor(logging.FATAL): self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
+        if self.isEnabledFor(logging.FATAL): self._log(logging.FATAL, cf.bold_red(msg), args, **kwargs)
 
     def prank_root(self, msg:str, color:str='', root=0, *args, **kwargs):
         '''print with rank. If color is not specified, use the color format corresponding to the rank'''
         if self.rank != root: return
         if not self.isEnabledFor(self.PRANK): return
         color = getattr(cf, color) if color else self.default_color
         self._log(self.PRANK, color(msg), args, **kwargs)
@@ -122,24 +122,24 @@
         '''print with rank. If color is not specified, use the color format corresponding to the rank'''
         if self.rank != root: return
         if not self.isEnabledFor(self.DEBUG): return
         color = getattr(cf, color) if color else self.default_color
         self._log(self.DEBUG, color(msg), args, **kwargs)
     def info_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        if self.isEnabledFor(logging.INFO): self._log(logging.INFO, cf.green(msg), args, kwargs)
+        if self.isEnabledFor(logging.INFO): self._log(logging.INFO, cf.green(msg), args, **kwargs)
     def warn_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        if self.isEnabledFor(logging.WARN): self._log(logging.WARN, cf.yellow(msg), args, kwargs)
+        if self.isEnabledFor(logging.WARN): self._log(logging.WARN, cf.yellow(msg), args, **kwargs)
     def error_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        if self.isEnabledFor(logging.ERROR): self._log(logging.ERROR, cf.red(msg), args, kwargs)
+        if self.isEnabledFor(logging.ERROR): self._log(logging.ERROR, cf.red(msg), args, **kwargs)
     def fatal_root(self, msg:str, root=0, *args, **kwargs):
         if self.rank != root: return
-        if self.isEnabledFor(logging.FATAL): self._log(logging.FATAL, cf.bold_red(msg), args, kwargs)
+        if self.isEnabledFor(logging.FATAL): self._log(logging.FATAL, cf.bold_red(msg), args, **kwargs)
         
     warning = warn
     critical = fatal
     warning_root = warn_root
     critical_root = fatal_root
     
 def get_level_from_env(logger_name:str, default_level="info"):
```

### Comparing `zq-tools-1.0.4/zq_tools/zq_tracing.py` & `zq-tools-1.0.5/zq_tools/zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.4/zq_tools.egg-info/PKG-INFO` & `zq-tools-1.0.5/zq_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of tools for zzqq2199
 Author: zzqq2199
 Author-email: zhouquanjs@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -19,14 +19,15 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
+- 1.0.5: fix bugs of `**kwargs` passing in `zq_logger`
 - 1.0.4: fix errors in logger.debug 
 - 1.0.3: make logger.debug to print without any color.
 - 1.0.2: fine grained control of different handlers
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
```

