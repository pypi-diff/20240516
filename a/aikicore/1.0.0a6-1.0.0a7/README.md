# Comparing `tmp/aikicore-1.0.0a6.tar.gz` & `tmp/aikicore-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aikicore-1.0.0a6.tar", last modified: Sun Apr 28 01:28:46 2024, max compression
+gzip compressed data, was "aikicore-1.0.0a7.tar", last modified: Sun Apr 28 01:33:58 2024, max compression
```

## Comparing `aikicore-1.0.0a6.tar` & `aikicore-1.0.0a7.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-28 01:28:46.590273 aikicore-1.0.0a6/
--rw-r--r--   0 ashatz     (501) staff       (20)     1509 2024-04-23 22:54:22.000000 aikicore-1.0.0a6/LICENSE
--rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-28 01:28:46.590058 aikicore-1.0.0a6/PKG-INFO
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-28 01:28:46.587841 aikicore-1.0.0a6/aikicore/
--rw-r--r--   0 ashatz     (501) staff       (20)     2434 2024-04-27 02:55:04.000000 aikicore-1.0.0a6/aikicore/__init__.py
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-28 01:28:46.589451 aikicore-1.0.0a6/aikicore/config/
--rw-r--r--   0 ashatz     (501) staff       (20)     3153 2024-04-27 03:05:30.000000 aikicore-1.0.0a6/aikicore/config/__init__.py
--rw-r--r--   0 ashatz     (501) staff       (20)      306 2024-04-23 22:57:31.000000 aikicore-1.0.0a6/aikicore/config/json.py
--rw-r--r--   0 ashatz     (501) staff       (20)      407 2024-04-23 22:57:31.000000 aikicore-1.0.0a6/aikicore/config/yaml.py
--rw-r--r--   0 ashatz     (501) staff       (20)      559 2024-04-27 02:47:15.000000 aikicore-1.0.0a6/aikicore/constants.py
-drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-28 01:28:46.589760 aikicore-1.0.0a6/aikicore.egg-info/
--rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-28 01:28:46.000000 aikicore-1.0.0a6/aikicore.egg-info/PKG-INFO
--rw-r--r--   0 ashatz     (501) staff       (20)      294 2024-04-28 01:28:46.000000 aikicore-1.0.0a6/aikicore.egg-info/SOURCES.txt
--rw-r--r--   0 ashatz     (501) staff       (20)        1 2024-04-28 01:28:46.000000 aikicore-1.0.0a6/aikicore.egg-info/dependency_links.txt
--rw-r--r--   0 ashatz     (501) staff       (20)       32 2024-04-28 01:28:46.000000 aikicore-1.0.0a6/aikicore.egg-info/requires.txt
--rw-r--r--   0 ashatz     (501) staff       (20)        9 2024-04-28 01:28:46.000000 aikicore-1.0.0a6/aikicore.egg-info/top_level.txt
--rw-r--r--   0 ashatz     (501) staff       (20)       38 2024-04-28 01:28:46.590330 aikicore-1.0.0a6/setup.cfg
--rw-r--r--   0 ashatz     (501) staff       (20)      657 2024-04-28 01:28:17.000000 aikicore-1.0.0a6/setup.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-28 01:33:58.960829 aikicore-1.0.0a7/
+-rw-r--r--   0 ashatz     (501) staff       (20)     1509 2024-04-23 22:54:22.000000 aikicore-1.0.0a7/LICENSE
+-rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-28 01:33:58.960645 aikicore-1.0.0a7/PKG-INFO
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-28 01:33:58.957087 aikicore-1.0.0a7/aikicore/
+-rw-r--r--   0 ashatz     (501) staff       (20)     2434 2024-04-27 02:55:04.000000 aikicore-1.0.0a7/aikicore/__init__.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-28 01:33:58.958585 aikicore-1.0.0a7/aikicore/config/
+-rw-r--r--   0 ashatz     (501) staff       (20)     3153 2024-04-27 03:05:30.000000 aikicore-1.0.0a7/aikicore/config/__init__.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      306 2024-04-23 22:57:31.000000 aikicore-1.0.0a7/aikicore/config/json.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      407 2024-04-23 22:57:31.000000 aikicore-1.0.0a7/aikicore/config/yaml.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      559 2024-04-27 02:47:15.000000 aikicore-1.0.0a7/aikicore/constants.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-28 01:33:58.960121 aikicore-1.0.0a7/aikicore/objects/
+-rw-r--r--   0 ashatz     (501) staff       (20)      250 2024-04-27 02:54:14.000000 aikicore-1.0.0a7/aikicore/objects/__init__.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      575 2024-04-24 01:05:56.000000 aikicore-1.0.0a7/aikicore/objects/container.py
+-rw-r--r--   0 ashatz     (501) staff       (20)      395 2024-04-23 22:57:31.000000 aikicore-1.0.0a7/aikicore/objects/domain.py
+-rw-r--r--   0 ashatz     (501) staff       (20)     1784 2024-04-25 22:40:31.000000 aikicore-1.0.0a7/aikicore/objects/error.py
+-rw-r--r--   0 ashatz     (501) staff       (20)     5634 2024-04-28 01:28:02.000000 aikicore-1.0.0a7/aikicore/objects/routing.py
+drwxr-xr-x   0 ashatz     (501) staff       (20)        0 2024-04-28 01:33:58.960441 aikicore-1.0.0a7/aikicore.egg-info/
+-rw-r--r--   0 ashatz     (501) staff       (20)      391 2024-04-28 01:33:58.000000 aikicore-1.0.0a7/aikicore.egg-info/PKG-INFO
+-rw-r--r--   0 ashatz     (501) staff       (20)      434 2024-04-28 01:33:58.000000 aikicore-1.0.0a7/aikicore.egg-info/SOURCES.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)        1 2024-04-28 01:33:58.000000 aikicore-1.0.0a7/aikicore.egg-info/dependency_links.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)       32 2024-04-28 01:33:58.000000 aikicore-1.0.0a7/aikicore.egg-info/requires.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)        9 2024-04-28 01:33:58.000000 aikicore-1.0.0a7/aikicore.egg-info/top_level.txt
+-rw-r--r--   0 ashatz     (501) staff       (20)       38 2024-04-28 01:33:58.960872 aikicore-1.0.0a7/setup.cfg
+-rw-r--r--   0 ashatz     (501) staff       (20)      685 2024-04-28 01:33:52.000000 aikicore-1.0.0a7/setup.py
```

### Comparing `aikicore-1.0.0a6/LICENSE` & `aikicore-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a6/aikicore/__init__.py` & `aikicore-1.0.0a7/aikicore/__init__.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a6/aikicore/config/__init__.py` & `aikicore-1.0.0a7/aikicore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a6/aikicore/constants.py` & `aikicore-1.0.0a7/aikicore/constants.py`

 * *Files identical despite different names*

### Comparing `aikicore-1.0.0a6/setup.py` & `aikicore-1.0.0a7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 config = {
     'description': 'The Core Library for the Spirit of Harmony',
     'author': 'Andrew Shatz',
     'url': r'https://github.com/Great-Strength-Studios/aikicore',
     'download_url': r'https://github.com/Great-Strength-Studios/aikicore',
     'author_email': 'andrew@greatstrength.me',
-    'version': '1.0.0-alpha.6',
+    'version': '1.0.0-alpha.7',
     'license': 'BSD 3',
     'install_requires': [
         'schematics>=2.1.1',
         'pyyaml>=6.0.1'
     ],
     'packages': [
         'aikicore',
         'aikicore.config',
+        'aikicore.objects',
     ],    
     'scripts': [],
     'name': 'aikicore'
 }
 
 setup(**config)
```

