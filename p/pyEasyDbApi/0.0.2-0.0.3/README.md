# Comparing `tmp/pyeasydbapi-0.0.2.tar.gz` & `tmp/pyeasydbapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasydbapi-0.0.2.tar", last modified: Thu May 16 21:15:15 2024, max compression
+gzip compressed data, was "pyeasydbapi-0.0.3.tar", last modified: Thu May 16 21:18:49 2024, max compression
```

## Comparing `pyeasydbapi-0.0.2.tar` & `pyeasydbapi-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-16 21:15:15.005440 pyeasydbapi-0.0.2/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.0.2/LICENSE
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      477 2024-05-16 21:15:15.005440 pyeasydbapi-0.0.2/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       49 2024-05-16 20:48:10.000000 pyeasydbapi-0.0.2/README.md
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-16 21:15:15.004440 pyeasydbapi-0.0.2/package/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       36 2024-05-16 20:46:11.000000 pyeasydbapi-0.0.2/package/__init__.py
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     3625 2024-05-16 20:32:12.000000 pyeasydbapi-0.0.2/package/main.py
-drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-16 21:15:15.005440 pyeasydbapi-0.0.2/pyEasyDbApi.egg-info/
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      477 2024-05-16 21:15:14.000000 pyeasydbapi-0.0.2/pyEasyDbApi.egg-info/PKG-INFO
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      212 2024-05-16 21:15:14.000000 pyeasydbapi-0.0.2/pyEasyDbApi.egg-info/SOURCES.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-16 21:15:14.000000 pyeasydbapi-0.0.2/pyEasyDbApi.egg-info/dependency_links.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        8 2024-05-16 21:15:14.000000 pyeasydbapi-0.0.2/pyEasyDbApi.egg-info/top_level.txt
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-16 21:15:15.005440 pyeasydbapi-0.0.2/setup.cfg
--rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-16 21:10:53.000000 pyeasydbapi-0.0.2/setup.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-16 21:18:49.588386 pyeasydbapi-0.0.3/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       12 2024-05-16 20:46:59.000000 pyeasydbapi-0.0.3/LICENSE
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      473 2024-05-16 21:18:49.588386 pyeasydbapi-0.0.3/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       45 2024-05-16 21:18:47.000000 pyeasydbapi-0.0.3/README.md
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-16 21:18:49.588386 pyeasydbapi-0.0.3/SimpleDB/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       36 2024-05-16 20:46:11.000000 pyeasydbapi-0.0.3/SimpleDB/__init__.py
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)     3625 2024-05-16 20:32:12.000000 pyeasydbapi-0.0.3/SimpleDB/main.py
+drwxr-xr-x   0 dimaluts  (1000) dimaluts  (1000)        0 2024-05-16 21:18:49.588386 pyeasydbapi-0.0.3/pyEasyDbApi.egg-info/
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      473 2024-05-16 21:18:49.000000 pyeasydbapi-0.0.3/pyEasyDbApi.egg-info/PKG-INFO
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      214 2024-05-16 21:18:49.000000 pyeasydbapi-0.0.3/pyEasyDbApi.egg-info/SOURCES.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        1 2024-05-16 21:18:49.000000 pyeasydbapi-0.0.3/pyEasyDbApi.egg-info/dependency_links.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)        9 2024-05-16 21:18:49.000000 pyeasydbapi-0.0.3/pyEasyDbApi.egg-info/top_level.txt
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)       38 2024-05-16 21:18:49.589386 pyeasydbapi-0.0.3/setup.cfg
+-rw-r--r--   0 dimaluts  (1000) dimaluts  (1000)      704 2024-05-16 21:18:47.000000 pyeasydbapi-0.0.3/setup.py
```

### Comparing `pyeasydbapi-0.0.2/package/main.py` & `pyeasydbapi-0.0.3/SimpleDB/main.py`

 * *Files identical despite different names*

### Comparing `pyeasydbapi-0.0.2/setup.py` & `pyeasydbapi-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='pyEasyDbApi',
-    version='0.0.2',
+    version='0.0.3',
     author='n1grtr33x',
     author_email='dmitroluc7@gmail.com',
     description='Simple DataBase to use',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/n1grtr33x',
     packages=find_packages(),
```
