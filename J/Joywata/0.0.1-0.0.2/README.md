# Comparing `tmp/Joywata-0.0.1.tar.gz` & `tmp/Joywata-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Joywata-0.0.1.tar", last modified: Thu May 16 06:14:55 2024, max compression
+gzip compressed data, was "Joywata-0.0.2.tar", last modified: Thu May 16 06:52:02 2024, max compression
```

## Comparing `Joywata-0.0.1.tar` & `Joywata-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 06:14:55.392688 Joywata-0.0.1/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 06:14:55.390508 Joywata-0.0.1/Joywata/
--rwxrwxrwx   0 root         (0) root         (0)       39 2024-05-16 06:14:47.000000 Joywata-0.0.1/Joywata/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3470 2024-05-16 06:10:54.000000 Joywata-0.0.1/Joywata/console.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 06:14:55.391990 Joywata-0.0.1/Joywata.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      595 2024-05-16 06:14:55.000000 Joywata-0.0.1/Joywata.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      215 2024-05-16 06:14:55.000000 Joywata-0.0.1/Joywata.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-16 06:14:55.000000 Joywata-0.0.1/Joywata.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       54 2024-05-16 06:14:55.000000 Joywata-0.0.1/Joywata.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2024-05-16 06:14:55.000000 Joywata-0.0.1/Joywata.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      595 2024-05-16 06:14:55.392395 Joywata-0.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       82 2024-05-16 06:14:47.000000 Joywata-0.0.1/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-16 06:14:55.392788 Joywata-0.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1763 2024-05-16 06:14:47.000000 Joywata-0.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 06:52:02.737455 Joywata-0.0.2/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 06:52:02.736142 Joywata-0.0.2/Joywata/
+-rwxrwxrwx   0 root         (0) root         (0)       39 2024-05-16 06:14:47.000000 Joywata-0.0.2/Joywata/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2983 2024-05-16 06:45:31.000000 Joywata-0.0.2/Joywata/console.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 06:52:02.737020 Joywata-0.0.2/Joywata.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      615 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      215 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       54 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      615 2024-05-16 06:52:02.737319 Joywata-0.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-05-16 06:50:19.000000 Joywata-0.0.2/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-16 06:52:02.737527 Joywata-0.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1760 2024-05-16 06:50:53.000000 Joywata-0.0.2/setup.py
```

### Comparing `Joywata-0.0.1/Joywata.egg-info/PKG-INFO` & `Joywata-0.0.2/Joywata.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Joywata
-Version: 0.0.1
-Summary: wangtao tools
+Version: 0.0.2
+Summary: wata tools
 Home-page: 
 Author: wangtao
 Author-email: 1083719817@qq.com
 Maintainer: wangtao
 Maintainer-email: 1083719817@qq.com
 License: MIT License
 Platform: Windows
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 
 # JOYWATA
-
+wata's terminal tools
 
 发布:
 ```
 python setup.py sdist bdist_wheel
 twine upload dist/*
 ```
+
+
```

### Comparing `Joywata-0.0.1/PKG-INFO` & `Joywata-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Joywata
-Version: 0.0.1
-Summary: wangtao tools
+Version: 0.0.2
+Summary: wata tools
 Home-page: 
 Author: wangtao
 Author-email: 1083719817@qq.com
 Maintainer: wangtao
 Maintainer-email: 1083719817@qq.com
 License: MIT License
 Platform: Windows
@@ -14,14 +14,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 
 # JOYWATA
-
+wata's terminal tools
 
 发布:
 ```
 python setup.py sdist bdist_wheel
 twine upload dist/*
 ```
+
+
```

### Comparing `Joywata-0.0.1/setup.py` & `Joywata-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 manylinux1_x86_64: 适用于符合ManyLinux规范的x86_64 Linux系统。
 win_amd64: 适用于64位Windows系统。
 macosx_10_9_x86_64: 适用于OS X 10.9及以上版本的x86_64 Mac系统
 '''
 
 setup(
     name='Joywata',  # 包名
-    version='0.0.1',  # 版本
-    description="wangtao tools",  # 包简介
+    version='0.0.2',  # 版本
+    description="wata tools",  # 包简介
     platforms=['Windows', 'Linux'],
     long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='wangtao',  # 作者
     author_email='1083719817@qq.com',  # 作者邮件
     maintainer='wangtao',  # 维护者
     maintainer_email='1083719817@qq.com',  # 维护者邮件
```

