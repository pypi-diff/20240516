# Comparing `tmp/tsc-cfg-0.2.tar.gz` & `tmp/tsc-cfg-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-cfg-0.2.tar", last modified: Sun Jan 28 08:37:21 2024, max compression
+gzip compressed data, was "tsc-cfg-0.3.tar", last modified: Thu Feb 29 07:54:53 2024, max compression
```

## Comparing `tsc-cfg-0.2.tar` & `tsc-cfg-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0     1024 users      (100)        0 2024-01-28 08:37:21.739388 tsc-cfg-0.2/
--rwxrwxrwx   0     1024 users      (100)    35149 2024-01-09 07:05:44.000000 tsc-cfg-0.2/LICENSE
--rwxrwxrwx   0     1024 users      (100)      966 2024-01-28 08:37:21.738388 tsc-cfg-0.2/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)       38 2024-01-28 08:37:21.740388 tsc-cfg-0.2/setup.cfg
--rwxrwxrwx   0     1024 users      (100)     1150 2024-01-16 05:42:00.000000 tsc-cfg-0.2/setup.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-01-28 08:37:21.725388 tsc-cfg-0.2/tsc_cfg/
--rwxrwxrwx   0     1024 users      (100)      245 2024-01-16 05:41:54.000000 tsc-cfg-0.2/tsc_cfg/__init__.py
--rwxrwxrwx   0     1024 users      (100)      948 2024-01-09 06:00:22.000000 tsc-cfg-0.2/tsc_cfg/cfg_utils.py
--rwxrwxrwx   0     1024 users      (100)    16298 2024-01-09 06:44:10.000000 tsc-cfg-0.2/tsc_cfg/global_info.py
--rwxrwxrwx   0     1024 users      (100)    23507 2024-01-28 08:36:31.000000 tsc-cfg-0.2/tsc_cfg/py_static_cfg.py
--rwxrwxrwx   0     1024 users      (100)     4239 2024-01-09 06:44:30.000000 tsc-cfg-0.2/tsc_cfg/test_global_info.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-01-28 08:37:21.736388 tsc-cfg-0.2/tsc_cfg.egg-info/
--rwxrwxrwx   0     1024 users      (100)      966 2024-01-28 08:37:21.000000 tsc-cfg-0.2/tsc_cfg.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      287 2024-01-28 08:37:21.000000 tsc-cfg-0.2/tsc_cfg.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2024-01-28 08:37:21.000000 tsc-cfg-0.2/tsc_cfg.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)      114 2024-01-28 08:37:21.000000 tsc-cfg-0.2/tsc_cfg.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)        8 2024-01-28 08:37:21.000000 tsc-cfg-0.2/tsc_cfg.egg-info/top_level.txt
+drwxrwxrwx   0     1024 users      (100)        0 2024-02-29 07:54:52.942942 tsc-cfg-0.3/
+-rwxrwxrwx   0     1024 users      (100)    35149 2024-01-09 07:05:44.000000 tsc-cfg-0.3/LICENSE
+-rwxrwxrwx   0     1024 users      (100)      966 2024-02-29 07:54:52.941943 tsc-cfg-0.3/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)       38 2024-02-29 07:54:52.943942 tsc-cfg-0.3/setup.cfg
+-rwxrwxrwx   0     1024 users      (100)     1150 2024-02-29 07:43:40.000000 tsc-cfg-0.3/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-02-29 07:54:52.923942 tsc-cfg-0.3/tsc_cfg/
+-rwxrwxrwx   0     1024 users      (100)      245 2024-01-16 05:41:54.000000 tsc-cfg-0.3/tsc_cfg/__init__.py
+-rwxrwxrwx   0     1024 users      (100)      948 2024-01-09 06:00:22.000000 tsc-cfg-0.3/tsc_cfg/cfg_utils.py
+-rwxrwxrwx   0     1024 users      (100)    16298 2024-01-09 06:44:10.000000 tsc-cfg-0.3/tsc_cfg/global_info.py
+-rwxrwxrwx   0     1024 users      (100)    23741 2024-02-29 07:51:56.000000 tsc-cfg-0.3/tsc_cfg/py_static_cfg.py
+-rwxrwxrwx   0     1024 users      (100)     4239 2024-01-09 06:44:30.000000 tsc-cfg-0.3/tsc_cfg/test_global_info.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-02-29 07:54:52.938943 tsc-cfg-0.3/tsc_cfg.egg-info/
+-rwxrwxrwx   0     1024 users      (100)      966 2024-02-29 07:54:52.000000 tsc-cfg-0.3/tsc_cfg.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      287 2024-02-29 07:54:52.000000 tsc-cfg-0.3/tsc_cfg.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2024-02-29 07:54:52.000000 tsc-cfg-0.3/tsc_cfg.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)      114 2024-02-29 07:54:52.000000 tsc-cfg-0.3/tsc_cfg.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)        8 2024-02-29 07:54:52.000000 tsc-cfg-0.3/tsc_cfg.egg-info/top_level.txt
```

### Comparing `tsc-cfg-0.2/LICENSE` & `tsc-cfg-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.2/PKG-INFO` & `tsc-cfg-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-cfg
-Version: 0.2
+Version: 0.3
 Summary: 自定义的配置文件
 Home-page: https://github.com/aitsc/tsc-cfg
 Author: aitsc
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tsc-cfg-0.2/setup.py` & `tsc-cfg-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = '教程: https://github.com/aitsc/tsc-cfg'
 
 setup(
     name='tsc-cfg',
-    version='0.2',
+    version='0.3',
     description="自定义的配置文件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='aitsc',
     license='GPLv3',
     url='https://github.com/aitsc/tsc-cfg',
     keywords='tools',
```

### Comparing `tsc-cfg-0.2/tsc_cfg/cfg_utils.py` & `tsc-cfg-0.3/tsc_cfg/cfg_utils.py`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.2/tsc_cfg/global_info.py` & `tsc-cfg-0.3/tsc_cfg/global_info.py`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.2/tsc_cfg/py_static_cfg.py` & `tsc-cfg-0.3/tsc_cfg/py_static_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,20 @@
             raise KeyError('KEY_NOT_FOUND')
         return False
 
     def __repr__(self) -> str:
         if self.use_raise:
             raise KeyError('KEY_NOT_FOUND')
         return "KEY_NOT_FOUND"
+    
+    def __getattr__(self, key: str) -> 'KeyNotFound':
+        """用点访问时，返回自身属性"""
+        if self.use_raise:
+            raise KeyError('KEY_NOT_FOUND')
+        return self
 
 
 KEY_NOT_FOUND = KeyNotFound()
 
 
 class SafeAttributeAccessor(type):
     def __getattr__(cls: 'Cfg', key: str) -> Union[Any, KeyNotFound]:
@@ -534,7 +540,8 @@
     
     print('---------meta test---------')
     # KEY_NOT_FOUND.use_raise = True
     print(MyClass.abcdefg, MyClass[-1])
     MyClass.abcdefg = MyClass['abcdefg'] = 1234
     print(MyClass['abcdefg'])
     print(MyClass['static_var1.a'])
+    print(KEY_NOT_FOUND.abc.asd)
```

### Comparing `tsc-cfg-0.2/tsc_cfg/test_global_info.py` & `tsc-cfg-0.3/tsc_cfg/test_global_info.py`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.2/tsc_cfg.egg-info/PKG-INFO` & `tsc-cfg-0.3/tsc_cfg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-cfg
-Version: 0.2
+Version: 0.3
 Summary: 自定义的配置文件
 Home-page: https://github.com/aitsc/tsc-cfg
 Author: aitsc
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

