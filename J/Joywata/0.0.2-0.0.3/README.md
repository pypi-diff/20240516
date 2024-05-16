# Comparing `tmp/Joywata-0.0.2.tar.gz` & `tmp/Joywata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Joywata-0.0.2.tar", last modified: Thu May 16 06:52:02 2024, max compression
+gzip compressed data, was "Joywata-0.0.3.tar", last modified: Thu May 16 07:05:35 2024, max compression
```

## Comparing `Joywata-0.0.2.tar` & `Joywata-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 06:52:02.737455 Joywata-0.0.2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 06:52:02.736142 Joywata-0.0.2/Joywata/
--rwxrwxrwx   0 root         (0) root         (0)       39 2024-05-16 06:14:47.000000 Joywata-0.0.2/Joywata/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2983 2024-05-16 06:45:31.000000 Joywata-0.0.2/Joywata/console.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 06:52:02.737020 Joywata-0.0.2/Joywata.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      615 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      215 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       54 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2024-05-16 06:52:02.000000 Joywata-0.0.2/Joywata.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      615 2024-05-16 06:52:02.737319 Joywata-0.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-05-16 06:50:19.000000 Joywata-0.0.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-16 06:52:02.737527 Joywata-0.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1760 2024-05-16 06:50:53.000000 Joywata-0.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 07:05:35.047810 Joywata-0.0.3/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 07:05:35.046265 Joywata-0.0.3/Joywata/
+-rwxrwxrwx   0 root         (0) root         (0)       39 2024-05-16 06:14:47.000000 Joywata-0.0.3/Joywata/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3045 2024-05-16 07:03:07.000000 Joywata-0.0.3/Joywata/console.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 07:05:35.047354 Joywata-0.0.3/Joywata.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      615 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      245 2024-05-16 07:05:35.000000 Joywata-0.0.3/Joywata.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       54 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      615 2024-05-16 07:05:35.047649 Joywata-0.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-05-16 06:50:19.000000 Joywata-0.0.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-16 07:05:35.047875 Joywata-0.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1769 2024-05-16 07:05:10.000000 Joywata-0.0.3/setup.py
```

### Comparing `Joywata-0.0.2/Joywata/console.py` & `Joywata-0.0.3/Joywata/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     table_list = [
         ['终端命令', '功能'],
         ['wata', 'Hello WATA !'],
         ['wata list', '列出wata终端命令'],
         ['wata install', '用清华源安装包'],
         ['wata unzip', 'ubuntu解压文件'],
         ['wata show_size', 'ubuntu查看子目录的大小'],
+        ['wata conda rm <env>', '删除conda中的env环境']
 
     ]
     print(tabulate(table_list, headers='firstrow', tablefmt='grid'))
 
 def pip_install_by_tsinghua(argv):
     assert argv.__len__() > 2
```

### Comparing `Joywata-0.0.2/Joywata.egg-info/PKG-INFO` & `Joywata-0.0.3/Joywata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Joywata
-Version: 0.0.2
+Version: 0.0.3
 Summary: wata tools
 Home-page: 
 Author: wangtao
 Author-email: 1083719817@qq.com
 Maintainer: wangtao
 Maintainer-email: 1083719817@qq.com
 License: MIT License
```

### Comparing `Joywata-0.0.2/PKG-INFO` & `Joywata-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Joywata
-Version: 0.0.2
+Version: 0.0.3
 Summary: wata tools
 Home-page: 
 Author: wangtao
 Author-email: 1083719817@qq.com
 Maintainer: wangtao
 Maintainer-email: 1083719817@qq.com
 License: MIT License
```

### Comparing `Joywata-0.0.2/setup.py` & `Joywata-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 any: 适用于任何平台的通用版本。
 manylinux1_x86_64: 适用于符合ManyLinux规范的x86_64 Linux系统。
 win_amd64: 适用于64位Windows系统。
 macosx_10_9_x86_64: 适用于OS X 10.9及以上版本的x86_64 Mac系统
 '''
 
 setup(
-    name='Joywata',  # 包名
-    version='0.0.2',  # 版本
+    name='Joywata', # 包名
+    version='0.0.3',  # 版本
     description="wata tools",  # 包简介
     platforms=['Windows', 'Linux'],
     long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='wangtao',  # 作者
     author_email='1083719817@qq.com',  # 作者邮件
     maintainer='wangtao',  # 维护者
@@ -34,14 +34,14 @@
             'python_tag': 'py3',
             'plat_name': 'any',
             'build_number': None,
             'dist_dir': None,
         }
     },
     python_requires='>=3.6',  # 设置python版本要求
-    install_requires=[],  # 安装所需要的库
+    install_requires=["tabulate"],  # 安装所需要的库
     entry_points={
         'console_scripts': [
             'wata=Joywata.console:wata_console',
         ],
     },  # 设置命令行工具(可不使用就可以注释掉)
 )
```

