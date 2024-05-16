# Comparing `tmp/cnparser-1.4.6.tar.gz` & `tmp/cnparser-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnparser-1.4.6.tar", last modified: Mon Apr  1 04:20:57 2024, max compression
+gzip compressed data, was "cnparser-1.5.0.tar", last modified: Thu May 16 00:11:40 2024, max compression
```

## Comparing `cnparser-1.4.6.tar` & `cnparser-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.221782 cnparser-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 04:20:45.000000 cnparser-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-01 04:20:57.221782 cnparser-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-01 04:20:45.000000 cnparser-1.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.217781 cnparser-1.4.6/cnparser/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.221782 cnparser-1.4.6/cnparser/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/config/file_id.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/config/header.json
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.221782 cnparser-1.4.6/cnparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 04:20:57.221782 cnparser-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-01 04:20:45.000000 cnparser-1.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.221782 cnparser-1.4.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:45.000000 cnparser-1.4.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-01 04:20:45.000000 cnparser-1.4.6/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.449327 cnparser-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-16 00:11:30.000000 cnparser-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-16 00:11:40.449327 cnparser-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-16 00:11:30.000000 cnparser-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.445327 cnparser-1.5.0/cnparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.449327 cnparser-1.5.0/cnparser/config/
+-rw-r--r--   0 runner    (1001) docker     (127)  1754761 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/config/eng_kana.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/config/file_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/config/header.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-16 00:11:30.000000 cnparser-1.5.0/cnparser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.449327 cnparser-1.5.0/cnparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 00:11:40.000000 cnparser-1.5.0/cnparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:11:40.449327 cnparser-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-16 00:11:30.000000 cnparser-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:40.449327 cnparser-1.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 00:11:30.000000 cnparser-1.5.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-16 00:11:30.000000 cnparser-1.5.0/test/test_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-16 00:11:30.000000 cnparser-1.5.0/test/test_load.py
```

### Comparing `cnparser-1.4.6/PKG-INFO` & `cnparser-1.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,59 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.4.6
+Version: 1.5.0
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
-License: Apache License 2.0
+License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
+Requires-Dist: pykakasi
 Requires-Dist: kanjize==1.5.0
 Requires-Dist: normalize-japanese-addresses==0.0.9
 
 # cnparser  
 [![Test](https://github.com/new-village/cnparser/actions/workflows/test.yaml/badge.svg)](https://github.com/new-village/cnparser/actions/workflows/test.yaml)  
 **cnparser** is a python library for loading and enrichment [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/en/) data that is provided from National Tax Agency Japan. cnparser only support to parse latest data now.   
   
-### Installation  
+## Installation  
 ----------------------
 cnparser is available on pip installation.
 ```
 $ python -m pip install cnparser
 ```
   
-#### GitHub Install
+### GitHub Install
 Installing the latest version from GitHub:  
 ```
 $ git clone https://github.com/new-village/cnparser
 $ cd cnparser
 $ python setup.py install
 ```
     
-### Usage
-----------------------
-Many properties are available once the cnparser object is created.  
-  
-#### Collect basic information (基本3情報)
-```python
->>> import cnparser
->>> cndata = cnparser.bulk_load("Shimane")
->>> print(cndata)
-[{'sequence_number': '1', 'corporate_number': '1000013050246', ...,  'hihyoji': '0'}, {...}]
+## Usage
+This section demonstrates how to use this library to load and process data from the National Tax Agency's [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/).
+
+### Direct Data Loading
+To load data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.
+To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be loaded. If you wish to load data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefecture](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)) like below: 
 ```
-  
-#### Enrich information from `bulk_load` result
-```python
 >>> import cnparser
->>> enriched = cnparser.bulk_enrich(cndata)
->>> print(enriched)
-[{'sequence_number': '1', ..., 'lat': 34.978982, 'lng': 132.525163, 'level': 3}, {...}]
+>>> df = cnparser.load("Shimane")
 ```
 
-#### Enrich information from downloaded CSV File
-```python
->>> import cnparser
->>> enriched = cnparser.bulk_enrich("path/to/data.csv")
->>> print(enriched)
-[{'sequence_number': '1', ..., 'lat': 34.978982, 'lng': 132.525163, 'level': 3}, {...}]
+### CSV Data Loading
+If you already have a downloaded CSV file, use the `read_csv` function. By passing the file path as an argument, you can obtain a DataFrame with headers from the CSV data.
 ```
-
-#### Enrich information to CSV file  
-You can export enriched data to CSV file directry by `export_file` option with file name.
-```python
 >>> import cnparser
->>> enriched = cnparser.bulk_enrich(cndata, export_file="path/to/export/data.csv")
+>>> df = cnparser.read_csv("path/to/data.csv")
 ```
 
-#### Enrich information to CSV file with downloaded api
-If you enrich massive data, You can use downloaded api.
-```
-$ cd /home/<USER>/
-$ curl -sL https://github.com/geolonia/japanese-addresses/archive/refs/heads/master.tar.gz | tar xvfz -
+## Tools
+### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
+This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
 ```
-  
-```python
->>> import cnparser
->>> enriched = cnparser.bulk_enrich(cndata, api_path="file:///home/<USER>/japanese-addresses-master/api/ja")
+$ cd /home/<USER>/analysis
+$ python enrich.py <FILE_PATH>
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cnparser-1.4.6/cnparser/config/header.json` & `cnparser-1.5.0/cnparser/config/header.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.4.6/cnparser/utility.py` & `cnparser-1.5.0/cnparser/utility.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 
 def load_api() -> str:
     resource_path = 'config/api/ja.json'  # パッケージ内のリソースへのパス
     if pkg_resources.resource_exists(__name__, resource_path):
         file_path = pkg_resources.resource_filename(__name__, resource_path)
         return 'file://' + file_path.replace('.json', '')
     else:
-        raise FileNotFoundError(f"No such file or directory: '{resource_path}'")
+        raise FileNotFoundError(f"No such file or directory: '{resource_path}'")
```

### Comparing `cnparser-1.4.6/cnparser.egg-info/PKG-INFO` & `cnparser-1.5.0/cnparser.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,59 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.4.6
+Version: 1.5.0
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
-License: Apache License 2.0
+License: GPLv3+
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: bs4
+Requires-Dist: pykakasi
 Requires-Dist: kanjize==1.5.0
 Requires-Dist: normalize-japanese-addresses==0.0.9
 
 # cnparser  
 [![Test](https://github.com/new-village/cnparser/actions/workflows/test.yaml/badge.svg)](https://github.com/new-village/cnparser/actions/workflows/test.yaml)  
 **cnparser** is a python library for loading and enrichment [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/en/) data that is provided from National Tax Agency Japan. cnparser only support to parse latest data now.   
   
-### Installation  
+## Installation  
 ----------------------
 cnparser is available on pip installation.
 ```
 $ python -m pip install cnparser
 ```
   
-#### GitHub Install
+### GitHub Install
 Installing the latest version from GitHub:  
 ```
 $ git clone https://github.com/new-village/cnparser
 $ cd cnparser
 $ python setup.py install
 ```
     
-### Usage
-----------------------
-Many properties are available once the cnparser object is created.  
-  
-#### Collect basic information (基本3情報)
-```python
->>> import cnparser
->>> cndata = cnparser.bulk_load("Shimane")
->>> print(cndata)
-[{'sequence_number': '1', 'corporate_number': '1000013050246', ...,  'hihyoji': '0'}, {...}]
+## Usage
+This section demonstrates how to use this library to load and process data from the National Tax Agency's [Corporate Number Publication Site](https://www.houjin-bangou.nta.go.jp/).
+
+### Direct Data Loading
+To load data for a specific prefecture, use the `load` function. By passing the prefecture name as an argument, you can obtain a DataFrame containing data for that prefecture.
+To execute the `load` function without specifying any arguments, data for all prefectures across Japan will be loaded. If you wish to load data for a specific prefecture, you must specify the prefecture name in Roman characters ([list of the supported prefecture](https://github.com/new-village/cnparser/blob/main/cnparser/config/file_id.json)) like below: 
 ```
-  
-#### Enrich information from `bulk_load` result
-```python
 >>> import cnparser
->>> enriched = cnparser.bulk_enrich(cndata)
->>> print(enriched)
-[{'sequence_number': '1', ..., 'lat': 34.978982, 'lng': 132.525163, 'level': 3}, {...}]
+>>> df = cnparser.load("Shimane")
 ```
 
-#### Enrich information from downloaded CSV File
-```python
->>> import cnparser
->>> enriched = cnparser.bulk_enrich("path/to/data.csv")
->>> print(enriched)
-[{'sequence_number': '1', ..., 'lat': 34.978982, 'lng': 132.525163, 'level': 3}, {...}]
+### CSV Data Loading
+If you already have a downloaded CSV file, use the `read_csv` function. By passing the file path as an argument, you can obtain a DataFrame with headers from the CSV data.
 ```
-
-#### Enrich information to CSV file  
-You can export enriched data to CSV file directry by `export_file` option with file name.
-```python
 >>> import cnparser
->>> enriched = cnparser.bulk_enrich(cndata, export_file="path/to/export/data.csv")
+>>> df = cnparser.read_csv("path/to/data.csv")
 ```
 
-#### Enrich information to CSV file with downloaded api
-If you enrich massive data, You can use downloaded api.
-```
-$ cd /home/<USER>/
-$ curl -sL https://github.com/geolonia/japanese-addresses/archive/refs/heads/master.tar.gz | tar xvfz -
+## Tools
+### import_dict.py: Bilingual Emacspeak Project (BEP) Dictionary Import Tool
+This tool imports the [BEP dictionary](https://fastapi.metacpan.org/source/MASH/Lingua-JA-Yomi-0.01/lib/Lingua/JA) and generates a dictionary file for use with cnparser. It processes the bilingual mappings from English to Kana, ensuring that cnparser can accurately handle and transform data involving these language elements.
 ```
-  
-```python
->>> import cnparser
->>> enriched = cnparser.bulk_enrich(cndata, api_path="file:///home/<USER>/japanese-addresses-master/api/ja")
+$ cd /home/<USER>/analysis
+$ python enrich.py <FILE_PATH>
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cnparser-1.4.6/setup.py` & `cnparser-1.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cnparser',
-    version='1.4.6',
+    version='1.5.0',
     author='new-village',
     url='https://github.com/new-village/cnparser',
     description='cnparser is a parser library of Corporate Number Publication Site data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    license = 'Apache License 2.0',
-    install_requires=['requests', 'bs4', 'kanjize==1.5.0', 'normalize-japanese-addresses==0.0.9'],
+    license = 'GPLv3+',
+    install_requires=['requests', 'bs4', 'pykakasi', 'kanjize==1.5.0', 'normalize-japanese-addresses==0.0.9'],
     packages=find_packages(),
     package_data={'': ['config/*.json']},
 )
```

