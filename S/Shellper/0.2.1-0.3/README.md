# Comparing `tmp/shellper-0.2.1.tar.gz` & `tmp/shellper-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellper-0.2.1.tar", last modified: Sun May 12 07:45:15 2024, max compression
+gzip compressed data, was "shellper-0.3.tar", last modified: Thu May 16 12:28:57 2024, max compression
```

## Comparing `shellper-0.2.1.tar` & `shellper-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 07:45:15.288016 shellper-0.2.1/
--rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      974 2024-05-12 07:45:15.275927 shellper-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-05-12 07:44:49.000000 shellper-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 07:45:15.275927 shellper-0.2.1/Shellper.egg-info/
--rw-rw-rw-   0        0        0      974 2024-05-12 07:45:15.000000 shellper-0.2.1/Shellper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-05-12 07:45:15.000000 shellper-0.2.1/Shellper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 07:45:15.000000 shellper-0.2.1/Shellper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-12 07:45:15.000000 shellper-0.2.1/Shellper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 07:45:15.000000 shellper-0.2.1/Shellper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 07:45:15.288016 shellper-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      845 2024-05-12 07:44:24.000000 shellper-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 07:45:15.260298 shellper-0.2.1/shellper/
--rw-rw-rw-   0        0        0      375 2024-05-12 07:43:35.000000 shellper-0.2.1/shellper/__init__.py
--rw-rw-rw-   0        0        0      677 2024-05-12 07:43:35.000000 shellper-0.2.1/shellper/inputs.py
--rw-rw-rw-   0        0        0     1676 2024-05-12 07:28:45.000000 shellper-0.2.1/shellper/log.py
--rw-rw-rw-   0        0        0      735 2024-05-12 07:22:51.000000 shellper-0.2.1/shellper/style.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:28:57.439381 shellper-0.3/
+-rw-rw-rw-   0        0        0    11357 2024-04-29 10:47:19.000000 shellper-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1055 2024-05-16 12:28:57.431782 shellper-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-05-16 12:28:36.000000 shellper-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 12:28:57.431782 shellper-0.3/Shellper.egg-info/
+-rw-rw-rw-   0        0        0     1055 2024-05-16 12:28:57.000000 shellper-0.3/Shellper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-16 12:28:57.000000 shellper-0.3/Shellper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:28:57.000000 shellper-0.3/Shellper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 12:28:57.000000 shellper-0.3/Shellper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:28:57.439381 shellper-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      833 2024-05-16 12:28:36.000000 shellper-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:28:57.421862 shellper-0.3/shellper/
+-rw-rw-rw-   0        0        0      376 2024-05-16 12:12:42.000000 shellper-0.3/shellper/__init__.py
+-rw-rw-rw-   0        0        0      378 2024-05-16 12:17:03.000000 shellper-0.3/shellper/datas.py
+-rw-rw-rw-   0        0        0      723 2024-05-16 12:01:56.000000 shellper-0.3/shellper/inputs.py
+-rw-rw-rw-   0        0        0     2639 2024-05-16 12:01:09.000000 shellper-0.3/shellper/log.py
+-rw-rw-rw-   0        0        0      735 2024-05-12 07:22:51.000000 shellper-0.3/shellper/style.py
```

### Comparing `shellper-0.2.1/LICENSE.txt` & `shellper-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shellper-0.2.1/PKG-INFO` & `shellper-0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.2.1
+Version: 0.3
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: requests>=2.31.0
 
 # Shellper
 
 A Python Library about shells.
 <br>It can help you create the better shell apps..
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
 
 ### Update Log:<br>
 
+v0.3 24/05/16 20:29: Update CMD Functions,Add Variable Supports,Add E_Type.<br>
 v0.2.1 24/05/12 15:45: Add CMD Functions.<br>
 v0.2 24/05/12 15:31: Removed Colorama Require.<br>
 v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.2.1/Shellper.egg-info/PKG-INFO` & `shellper-0.3/Shellper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: Shellper
-Version: 0.2.1
+Version: 0.3
 Summary: A Python Library for create shell apps.
 Home-page: https://gitee.com/ShawnMerry/Shellper
 Author: ShawnMerry
 Author-email: merrybili@163.com
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: requests>=2.31.0
 
 # Shellper
 
 A Python Library about shells.
 <br>It can help you create the better shell apps..
 
 #### [PyPI](https://pypi.org/project/Shellper)
 
 #### [Gitee](https://gitee.com/ShawnMerry/Shellper)
 
 ### Update Log:<br>
 
+v0.3 24/05/16 20:29: Update CMD Functions,Add Variable Supports,Add E_Type.<br>
 v0.2.1 24/05/12 15:45: Add CMD Functions.<br>
 v0.2 24/05/12 15:31: Removed Colorama Require.<br>
 v0.1 24/05/11: Initial Update.
```

### Comparing `shellper-0.2.1/setup.py` & `shellper-0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="Shellper",
-    version="0.2.1",
+    version="0.3",
     author="ShawnMerry",
     author_email="merrybili@163.com",
     description="A Python Library for create shell apps.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ShawnMerry/Shellper",
     packages=find_packages(),
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Internet"
     ],
-    python_requires=">=3",
-    install_requires=['requests>=2.31.0']
+    python_requires=">=3"
 )
```

### Comparing `shellper-0.2.1/shellper/log.py` & `shellper-0.3/shellper/log.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,61 @@
 from datetime import datetime
 from .style import *
 
 
-def info(name, message, show: bool = True):
+def info(name, message, show: bool = True, e_type: str = None):
     try:
         name = str(name)
         message = str(message)
     except TypeError:
-        raise ConvertError("Name or message must can convert to string")
+        raise ConvertError("Name or message must can convert to string.")
     date = datetime.now().strftime("%y/%m/%d %H:%M:%S")
-    print(f"{Style.BRIGHT}{date + ' ' if show else ''}[Info] {name}: {Style.NORMAL + message + Style.RESET}")
+    if e_type is not None:
+        print(f"{Style.BRIGHT}{date + ' ' if show else ''}[Info] {name}: {"{" + e_type + "}"}"
+              f" {Style.NORMAL + message + Style.RESET}")
+    else:
+        print(f"{Style.BRIGHT}{date + ' ' if show else ''}[Info] {name}: {Style.NORMAL + message + Style.RESET}")
 
 
-def warning(name, message, show: bool = True):
+def warning(name, message, show: bool = True, e_type: str = None):
     try:
         name = str(name)
         message = str(message)
     except TypeError:
-        raise ConvertError("Name or message must can convert to string")
+        raise ConvertError("Name or message must can convert to string.")
     date = datetime.now().strftime("%y/%m/%d %H:%M:%S")
-    print(
-        f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_YELLOW}[Warning] {name}: {Style.NORMAL + message + Style.RESET}")
+    if e_type is not None:
+        print(f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_YELLOW}[Warning] {name}: {"{" + e_type + "}"}"
+              f" {Style.NORMAL + message + Style.RESET}")
+    else:
+        print(f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_YELLOW}[Warning] {name}: "
+              f"{Style.NORMAL + message + Style.RESET}")
 
 
-def error(name, message, show: bool = True):
+def error(name, message, show: bool = True, e_type: str = None):
     try:
         name = str(name)
         message = str(message)
     except TypeError:
-        raise ConvertError("Name or message must can convert to string")
+        raise ConvertError("Name or message must can convert to string.")
     date = datetime.now().strftime("%y/%m/%d %H:%M:%S")
-    print(
-        f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_RED}[Error] {name}: {Style.NORMAL + message + Style.RESET}")
+    if e_type is not None:
+        print(f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_RED}[Error] {name}: {"{" + e_type + "}"}"
+              f" {Style.NORMAL + message + Style.RESET}")
+    else:
+        print(f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_RED}[Error] {name}: "
+              f"{Style.NORMAL + message + Style.RESET}")
 
 
-def debug(name, message, show: bool = True):
+def debug(name, message, show: bool = True, e_type: str = None):
     try:
         name = str(name)
         message = str(message)
     except TypeError:
-        raise ConvertError("Name or message must can convert to string")
+        raise ConvertError("Name or message must can convert to string.")
     date = datetime.now().strftime("%y/%m/%d %H:%M:%S")
-    print(
-        f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_BLUE}[Debug] {name}: {Style.NORMAL + message + Style.RESET}")
+    if e_type is not None:
+        print(f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_BLUE}[Debug] {name}: {"{" + e_type + "}"}"
+              f" {Style.NORMAL + message + Style.RESET}")
+    else:
+        print(f"{Style.BRIGHT}{date + ' ' if show else ''}{Style.LIGHT_BLUE}[Debug] {name}: "
+              f"{Style.NORMAL + message + Style.RESET}")
```

### Comparing `shellper-0.2.1/shellper/style.py` & `shellper-0.3/shellper/style.py`

 * *Files identical despite different names*

