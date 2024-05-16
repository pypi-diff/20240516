# Comparing `tmp/Joywata-0.0.3.tar.gz` & `tmp/Joywata-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Joywata-0.0.3.tar", last modified: Thu May 16 07:05:35 2024, max compression
+gzip compressed data, was "Joywata-0.0.4.tar", last modified: Thu May 16 07:16:01 2024, max compression
```

## Comparing `Joywata-0.0.3.tar` & `Joywata-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 07:05:35.047810 Joywata-0.0.3/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 07:05:35.046265 Joywata-0.0.3/Joywata/
--rwxrwxrwx   0 root         (0) root         (0)       39 2024-05-16 06:14:47.000000 Joywata-0.0.3/Joywata/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3045 2024-05-16 07:03:07.000000 Joywata-0.0.3/Joywata/console.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 07:05:35.047354 Joywata-0.0.3/Joywata.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      615 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      245 2024-05-16 07:05:35.000000 Joywata-0.0.3/Joywata.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       54 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)        9 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2024-05-16 07:05:34.000000 Joywata-0.0.3/Joywata.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      615 2024-05-16 07:05:35.047649 Joywata-0.0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-05-16 06:50:19.000000 Joywata-0.0.3/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-16 07:05:35.047875 Joywata-0.0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1769 2024-05-16 07:05:10.000000 Joywata-0.0.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 07:16:01.613087 Joywata-0.0.4/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 07:16:01.611563 Joywata-0.0.4/Joywata/
+-rwxrwxrwx   0 root         (0) root         (0)       39 2024-05-16 06:14:47.000000 Joywata-0.0.4/Joywata/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3147 2024-05-16 07:14:41.000000 Joywata-0.0.4/Joywata/console.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 07:16:01.612568 Joywata-0.0.4/Joywata.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      614 2024-05-16 07:16:01.000000 Joywata-0.0.4/Joywata.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      245 2024-05-16 07:16:01.000000 Joywata-0.0.4/Joywata.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-16 07:16:01.000000 Joywata-0.0.4/Joywata.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       54 2024-05-16 07:16:01.000000 Joywata-0.0.4/Joywata.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)        9 2024-05-16 07:16:01.000000 Joywata-0.0.4/Joywata.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        8 2024-05-16 07:16:01.000000 Joywata-0.0.4/Joywata.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      614 2024-05-16 07:16:01.612861 Joywata-0.0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-05-16 06:50:19.000000 Joywata-0.0.4/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-16 07:16:01.613147 Joywata-0.0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1771 2024-05-16 07:15:54.000000 Joywata-0.0.4/setup.py
```

### Comparing `Joywata-0.0.3/Joywata/console.py` & `Joywata-0.0.4/Joywata/console.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from pathlib import Path
 
 def wata_list(argv):
     assert argv.__len__() == 2, 'error command'
     table_list = [
         ['终端命令', '功能'],
-        ['wata', 'Hello WATA !'],
+        ['wata', 'Hello JOYWATA !'],
         ['wata list', '列出wata终端命令'],
         ['wata install', '用清华源安装包'],
         ['wata unzip', 'ubuntu解压文件'],
         ['wata show_size', 'ubuntu查看子目录的大小'],
         ['wata conda rm <env>', '删除conda中的env环境']
 
     ]
@@ -32,14 +32,15 @@
         os.system("pip uninstall " + package)
 
 def conda_cmd(argv):
     assert argv.__len__() > 3
     if argv[2] == "rm":
         print("conda rm " + argv[-1] + " --all")
         os.system("conda remove -n " + argv[-1] + " --all")
+
 def unzip(argv):
     user = '' if argv[1] == 'unzip' else 'sudo '
     assert argv.__len__() > 2
     zip_file = argv[2]
     zip_ext = Path(zip_file).suffix[1:]
     print(zip_ext)
     if zip_ext == "zip":
@@ -58,15 +59,15 @@
         print(user + "tar -xvf " + zip_file)
         os.system(user + "tar -xvf " + zip_file)
     else:
         print('Unable to decompress the file type temporarily')
 
 def wata_console():
     if sys.argv.__len__() == 1:
-        print("Hello WATA !")
+        print("Hello JOYWATA !")
         print('Enter "wata list" to view the function')
         return None
 
     cmd = sys.argv[1]
     if cmd == 'install' or cmd == 'uninstall':
         pip_install_by_tsinghua(sys.argv)
         return None
@@ -83,14 +84,18 @@
         wata_list(sys.argv)
         return None
 
     elif cmd == 'show_size':
         os.system("sudo du -h --max-depth=1")
         return None
 
+    elif cmd == 'cuda':
+        os.system("ls /usr/local/ | grep ^cuda-")
+        return None
+
     elif cmd == 'conda':
         conda_cmd(sys.argv)
         return None
     else:
         print("error command")
```

### Comparing `Joywata-0.0.3/Joywata.egg-info/PKG-INFO` & `Joywata-0.0.4/Joywata.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: Joywata
-Version: 0.0.3
+Version: 0.0.4
 Summary: wata tools
 Home-page: 
 Author: wangtao
 Author-email: 1083719817@qq.com
 Maintainer: wangtao
 Maintainer-email: 1083719817@qq.com
 License: MIT License
 Platform: Windows
 Platform: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Dist: tabulate
 
 # JOYWATA
 wata's terminal tools
 
 发布:
 ```
 python setup.py sdist bdist_wheel
 twine upload dist/*
 ```
-
-
```

### Comparing `Joywata-0.0.3/PKG-INFO` & `Joywata-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: Joywata
-Version: 0.0.3
+Version: 0.0.4
 Summary: wata tools
 Home-page: 
 Author: wangtao
 Author-email: 1083719817@qq.com
 Maintainer: wangtao
 Maintainer-email: 1083719817@qq.com
 License: MIT License
 Platform: Windows
 Platform: Linux
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Dist: tabulate
 
 # JOYWATA
 wata's terminal tools
 
 发布:
 ```
 python setup.py sdist bdist_wheel
 twine upload dist/*
 ```
-
-
```

### Comparing `Joywata-0.0.3/setup.py` & `Joywata-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 manylinux1_x86_64: 适用于符合ManyLinux规范的x86_64 Linux系统。
 win_amd64: 适用于64位Windows系统。
 macosx_10_9_x86_64: 适用于OS X 10.9及以上版本的x86_64 Mac系统
 '''
 
 setup(
     name='Joywata', # 包名
-    version='0.0.3',  # 版本
+    version='0.0.4',  # 版本
     description="wata tools",  # 包简介
     platforms=['Windows', 'Linux'],
     long_description=open('README.md').read(),  # 读取文件中介绍包的详细内容
     include_package_data=True,  # 是否允许上传资源文件
     author='wangtao',  # 作者
     author_email='1083719817@qq.com',  # 作者邮件
     maintainer='wangtao',  # 维护者
@@ -33,15 +33,15 @@
         'bdist_wheel': {
             'python_tag': 'py3',
             'plat_name': 'any',
             'build_number': None,
             'dist_dir': None,
         }
     },
-    python_requires='>=3.6',  # 设置python版本要求
+    # python_requires='>=3.6',  # 设置python版本要求
     install_requires=["tabulate"],  # 安装所需要的库
     entry_points={
         'console_scripts': [
             'wata=Joywata.console:wata_console',
         ],
     },  # 设置命令行工具(可不使用就可以注释掉)
 )
```

