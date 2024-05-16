# Comparing `tmp/cnparser-1.5.0.tar.gz` & `tmp/cnparser-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnparser-1.5.0.tar", last modified: Thu May 16 00:11:40 2024, max compression
+gzip compressed data, was "cnparser-1.5.1.tar", last modified: Thu May 16 00:14:50 2024, max compression
```

## Comparing `cnparser-1.5.0.tar` & `cnparser-1.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.449327 cnparser-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-16 00:11:30.000000 cnparser-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-16 00:11:40.449327 cnparser-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-16 00:11:30.000000 cnparser-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.445327 cnparser-1.5.0/cnparser/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.449327 cnparser-1.5.0/cnparser/config/
--rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/config/eng_kana.json
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/config/file_id.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/config/header.json
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.449327 cnparser-1.5.0/cnparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:11:40.449327 cnparser-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-16 00:11:30.000000 cnparser-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.449327 cnparser-1.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:30.000000 cnparser-1.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-16 00:11:30.000000 cnparser-1.5.0/test/test_enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-16 00:11:30.000000 cnparser-1.5.0/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:14:50.697077 cnparser-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-16 00:14:40.000000 cnparser-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-16 00:14:50.697077 cnparser-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-16 00:14:40.000000 cnparser-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:14:50.693077 cnparser-1.5.1/cnparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 00:14:40.000000 cnparser-1.5.1/cnparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:14:50.697077 cnparser-1.5.1/cnparser/config/
+-rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-16 00:14:40.000000 cnparser-1.5.1/cnparser/config/eng_kana.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-16 00:14:40.000000 cnparser-1.5.1/cnparser/config/file_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-16 00:14:40.000000 cnparser-1.5.1/cnparser/config/header.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-16 00:14:40.000000 cnparser-1.5.1/cnparser/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-16 00:14:40.000000 cnparser-1.5.1/cnparser/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-16 00:14:40.000000 cnparser-1.5.1/cnparser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:14:50.697077 cnparser-1.5.1/cnparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-16 00:14:50.000000 cnparser-1.5.1/cnparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-16 00:14:50.000000 cnparser-1.5.1/cnparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:14:50.000000 cnparser-1.5.1/cnparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 00:14:50.000000 cnparser-1.5.1/cnparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 00:14:50.000000 cnparser-1.5.1/cnparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:14:50.697077 cnparser-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 00:14:40.000000 cnparser-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:14:50.697077 cnparser-1.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 00:14:40.000000 cnparser-1.5.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-16 00:14:40.000000 cnparser-1.5.1/test/test_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-16 00:14:40.000000 cnparser-1.5.1/test/test_load.py
```

### Comparing `cnparser-1.5.0/LICENSE` & `cnparser-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.0/PKG-INFO` & `cnparser-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.5.0
+Version: 1.5.1
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
+Requires-Dist: pandas
 Requires-Dist: pykakasi
 Requires-Dist: kanjize==1.5.0
 Requires-Dist: normalize-japanese-addresses==0.0.9
 
 # cnparser  
 [![Test](https://github.com/new-village/cnparser/actions/workflows/test.yaml/badge.svg)](https://github.com/new-village/cnparser/actions/workflows/test.yaml)  
 **cnparser** is a python library for loading and enrichment [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/en/) data that is provided from National Tax Agency Japan. cnparser only support to parse latest data now.
```

### Comparing `cnparser-1.5.0/README.md` & `cnparser-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.0/cnparser/config/eng_kana.json` & `cnparser-1.5.1/cnparser/config/eng_kana.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.0/cnparser/config/file_id.json` & `cnparser-1.5.1/cnparser/config/file_id.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.0/cnparser/config/header.json` & `cnparser-1.5.1/cnparser/config/header.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.0/cnparser/enrich.py` & `cnparser-1.5.1/cnparser/enrich.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.0/cnparser/load.py` & `cnparser-1.5.1/cnparser/load.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.0/cnparser/utility.py` & `cnparser-1.5.1/cnparser/utility.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.0/cnparser.egg-info/PKG-INFO` & `cnparser-1.5.1/cnparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.5.0
+Version: 1.5.1
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
+Requires-Dist: pandas
 Requires-Dist: pykakasi
 Requires-Dist: kanjize==1.5.0
 Requires-Dist: normalize-japanese-addresses==0.0.9
 
 # cnparser  
 [![Test](https://github.com/new-village/cnparser/actions/workflows/test.yaml/badge.svg)](https://github.com/new-village/cnparser/actions/workflows/test.yaml)  
 **cnparser** is a python library for loading and enrichment [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/en/) data that is provided from National Tax Agency Japan. cnparser only support to parse latest data now.
```

### Comparing `cnparser-1.5.0/setup.py` & `cnparser-1.5.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cnparser',
-    version='1.5.0',
+    version='1.5.1',
     author='new-village',
     url='https://github.com/new-village/cnparser',
     description='cnparser is a parser library of Corporate Number Publication Site data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'GPLv3+',
-    install_requires=['requests', 'bs4', 'pykakasi', 'kanjize==1.5.0', 'normalize-japanese-addresses==0.0.9'],
+    install_requires=['requests', 'bs4', 'pandas', 'pykakasi', 'kanjize==1.5.0', 'normalize-japanese-addresses==0.0.9'],
     packages=find_packages(),
     package_data={'': ['config/*.json']},
 )
```

### Comparing `cnparser-1.5.0/test/test_enrich.py` & `cnparser-1.5.1/test/test_enrich.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.5.0/test/test_load.py` & `cnparser-1.5.1/test/test_load.py`

 * *Files identical despite different names*

