# Comparing `tmp/pymonit-1.3.12.tar.gz` & `tmp/pymonit-1.3.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonit-1.3.12.tar", last modified: Wed May 15 22:02:45 2024, max compression
+gzip compressed data, was "pymonit-1.3.13.tar", last modified: Wed May 15 22:20:13 2024, max compression
```

## Comparing `pymonit-1.3.12.tar` & `pymonit-1.3.13.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:02:45.752447 pymonit-1.3.12/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.12/LICENSE
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2398 2024-05-15 22:02:45.752447 pymonit-1.3.12/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1762 2024-05-15 22:01:11.000000 pymonit-1.3.12/README.md
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:02:45.749113 pymonit-1.3.12/pymonit/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.12/pymonit/__init__.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.12/pymonit/config.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      788 2024-05-15 21:57:36.000000 pymonit-1.3.12/pymonit/core.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-15 21:54:39.000000 pymonit-1.3.12/pymonit/database.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.12/pymonit/error.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3147 2024-05-15 21:54:50.000000 pymonit-1.3.12/pymonit/func.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.12/pymonit/log2file.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.12/pymonit/logger.py
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.12/pymonit/verify_env.py
-drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:02:45.752447 pymonit-1.3.12/pymonit.egg-info/
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2398 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/PKG-INFO
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      347 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/SOURCES.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/dependency_links.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/requires.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)        8 2024-05-15 22:02:45.000000 pymonit-1.3.12/pymonit.egg-info/top_level.txt
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-15 22:02:45.752447 pymonit-1.3.12/setup.cfg
--rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-15 22:02:02.000000 pymonit-1.3.12/setup.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:20:13.145824 pymonit-1.3.13/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1064 2024-04-22 01:06:10.000000 pymonit-1.3.13/LICENSE
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2398 2024-05-15 22:20:13.145824 pymonit-1.3.13/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1762 2024-05-15 22:01:11.000000 pymonit-1.3.13/README.md
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:20:13.145824 pymonit-1.3.13/pymonit/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        0 2024-04-22 01:06:10.000000 pymonit-1.3.13/pymonit/__init__.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      922 2024-04-30 01:09:27.000000 pymonit-1.3.13/pymonit/config.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      788 2024-05-15 21:57:36.000000 pymonit-1.3.13/pymonit/core.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1594 2024-05-15 21:54:39.000000 pymonit-1.3.13/pymonit/database.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      227 2024-04-25 22:34:06.000000 pymonit-1.3.13/pymonit/error.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     3147 2024-05-15 21:54:50.000000 pymonit-1.3.13/pymonit/func.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     1831 2024-04-22 23:15:08.000000 pymonit-1.3.13/pymonit/log2file.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2569 2024-04-22 23:04:24.000000 pymonit-1.3.13/pymonit/logger.py
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      272 2024-05-15 21:55:05.000000 pymonit-1.3.13/pymonit/verify_env.py
+drwxr-xr-x   0 arktnld   (1000) arktnld   (1000)        0 2024-05-15 22:20:13.145824 pymonit-1.3.13/pymonit.egg-info/
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)     2398 2024-05-15 22:20:12.000000 pymonit-1.3.13/pymonit.egg-info/PKG-INFO
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      347 2024-05-15 22:20:13.000000 pymonit-1.3.13/pymonit.egg-info/SOURCES.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        1 2024-05-15 22:20:12.000000 pymonit-1.3.13/pymonit.egg-info/dependency_links.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       40 2024-05-15 22:20:12.000000 pymonit-1.3.13/pymonit.egg-info/requires.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)        8 2024-05-15 22:20:12.000000 pymonit-1.3.13/pymonit.egg-info/top_level.txt
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)       38 2024-05-15 22:20:13.145824 pymonit-1.3.13/setup.cfg
+-rw-r--r--   0 arktnld   (1000) arktnld   (1000)      866 2024-05-15 22:17:54.000000 pymonit-1.3.13/setup.py
```

### Comparing `pymonit-1.3.12/LICENSE` & `pymonit-1.3.13/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.12/PKG-INFO` & `pymonit-1.3.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.12
+Version: 1.3.13
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymonit-1.3.12/README.md` & `pymonit-1.3.13/README.md`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.12/pymonit/config.py` & `pymonit-1.3.13/pymonit/config.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.12/pymonit/core.py` & `pymonit-1.3.13/pymonit/core.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.12/pymonit/database.py` & `pymonit-1.3.13/pymonit/database.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.12/pymonit/func.py` & `pymonit-1.3.13/pymonit/func.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.12/pymonit/log2file.py` & `pymonit-1.3.13/pymonit/log2file.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.12/pymonit/logger.py` & `pymonit-1.3.13/pymonit/logger.py`

 * *Files identical despite different names*

### Comparing `pymonit-1.3.12/pymonit.egg-info/PKG-INFO` & `pymonit-1.3.13/pymonit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonit
-Version: 1.3.12
+Version: 1.3.13
 Summary: Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados
 Home-page: https://github.com/arktnld/monit
 Author: arktnld
 Author-email: arktnld@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pymonit-1.3.12/setup.py` & `pymonit-1.3.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import pathlib
 
 setup(
     name='pymonit',
-    version='1.3.12',
+    version='1.3.13',
     description='Programa de monitoramento de código python, desenvolvido para ser utilizado pelas funcionário da Agência de dados',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     author='arktnld',
     author_email='arktnld@gmail.com',
     url='https://github.com/arktnld/monit',
     license='MIT',
```

