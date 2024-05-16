# Comparing `tmp/cnparser-1.4.5.tar.gz` & `tmp/cnparser-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnparser-1.4.5.tar", last modified: Mon Apr  1 03:55:37 2024, max compression
+gzip compressed data, was "cnparser-1.4.6.tar", last modified: Mon Apr  1 04:20:57 2024, max compression
```

## Comparing `cnparser-1.4.5.tar` & `cnparser-1.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:55:37.751819 cnparser-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 03:55:27.000000 cnparser-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-01 03:55:37.751819 cnparser-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-01 03:55:27.000000 cnparser-1.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:55:37.747819 cnparser-1.4.5/cnparser/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-01 03:55:27.000000 cnparser-1.4.5/cnparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:55:37.751819 cnparser-1.4.5/cnparser/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-01 03:55:27.000000 cnparser-1.4.5/cnparser/config/file_id.json
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-01 03:55:27.000000 cnparser-1.4.5/cnparser/config/header.json
--rw-r--r--   0 runner    (1001) docker     (127)     7469 2024-04-01 03:55:27.000000 cnparser-1.4.5/cnparser/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-01 03:55:27.000000 cnparser-1.4.5/cnparser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:55:37.751819 cnparser-1.4.5/cnparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-01 03:55:37.000000 cnparser-1.4.5/cnparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 03:55:37.000000 cnparser-1.4.5/cnparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 03:55:37.000000 cnparser-1.4.5/cnparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 03:55:37.000000 cnparser-1.4.5/cnparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 03:55:37.000000 cnparser-1.4.5/cnparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 03:55:37.751819 cnparser-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-01 03:55:27.000000 cnparser-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 03:55:37.751819 cnparser-1.4.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 03:55:27.000000 cnparser-1.4.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-01 03:55:27.000000 cnparser-1.4.5/test/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.221782 cnparser-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 04:20:45.000000 cnparser-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-01 04:20:57.221782 cnparser-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-01 04:20:45.000000 cnparser-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.217781 cnparser-1.4.6/cnparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.221782 cnparser-1.4.6/cnparser/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/config/file_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/config/header.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-01 04:20:45.000000 cnparser-1.4.6/cnparser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.221782 cnparser-1.4.6/cnparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 04:20:57.000000 cnparser-1.4.6/cnparser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 04:20:57.221782 cnparser-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-01 04:20:45.000000 cnparser-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:57.221782 cnparser-1.4.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 04:20:45.000000 cnparser-1.4.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-01 04:20:45.000000 cnparser-1.4.6/test/test_load.py
```

### Comparing `cnparser-1.4.5/LICENSE` & `cnparser-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cnparser-1.4.5/PKG-INFO` & `cnparser-1.4.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.4.5
+Version: 1.4.6
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -61,7 +61,19 @@
 
 #### Enrich information to CSV file  
 You can export enriched data to CSV file directry by `export_file` option with file name.
 ```python
 >>> import cnparser
 >>> enriched = cnparser.bulk_enrich(cndata, export_file="path/to/export/data.csv")
 ```
+
+#### Enrich information to CSV file with downloaded api
+If you enrich massive data, You can use downloaded api.
+```
+$ cd /home/<USER>/
+$ curl -sL https://github.com/geolonia/japanese-addresses/archive/refs/heads/master.tar.gz | tar xvfz -
+```
+  
+```python
+>>> import cnparser
+>>> enriched = cnparser.bulk_enrich(cndata, api_path="file:///home/<USER>/japanese-addresses-master/api/ja")
+```
```

### Comparing `cnparser-1.4.5/README.md` & `cnparser-1.4.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -47,7 +47,19 @@
 
 #### Enrich information to CSV file  
 You can export enriched data to CSV file directry by `export_file` option with file name.
 ```python
 >>> import cnparser
 >>> enriched = cnparser.bulk_enrich(cndata, export_file="path/to/export/data.csv")
 ```
+
+#### Enrich information to CSV file with downloaded api
+If you enrich massive data, You can use downloaded api.
+```
+$ cd /home/<USER>/
+$ curl -sL https://github.com/geolonia/japanese-addresses/archive/refs/heads/master.tar.gz | tar xvfz -
+```
+  
+```python
+>>> import cnparser
+>>> enriched = cnparser.bulk_enrich(cndata, api_path="file:///home/<USER>/japanese-addresses-master/api/ja")
+```
```

### Comparing `cnparser-1.4.5/cnparser/config/file_id.json` & `cnparser-1.4.6/cnparser/config/file_id.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.4.5/cnparser/config/header.json` & `cnparser-1.4.6/cnparser/config/header.json`

 * *Files identical despite different names*

### Comparing `cnparser-1.4.5/cnparser/load.py` & `cnparser-1.4.6/cnparser/load.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,28 +21,30 @@
     """ Load Corporate Number Publication Site data.
     :param prefecture: prefecture name such as ALL, tokyo, tottori and shizuoka
     :return: :class:`List <list>` object
     """
     loader = ZipLoader()
     return loader.bulk_load(_prefecture_2_file_id(prefecture))
 
-def bulk_enrich(data, export_file=None):
+def bulk_enrich(data, export_file=None, api_path=None):
     """ 
     Enriches the data from the Corporate Number Publication Site.
     Accepts either a path to a CSV file or a list of data, and returns a list of data with normalized address information.
 
     :param data: Path to a CSV file or a list of corporate data
+    :param export_file: Optional; if provided, the enriched data will be written to this file
+    :param api_path: Optional; if provided, it will be used as the endpoint for the normalize function
     :return: A list of corporate data with normalized address information
     """
     if isinstance(data, str) and ".csv" in data:
         data = _read_csv_file(data)
     elif not isinstance(data, list):
         raise ValueError("Invalid argument type. Argument must be a .csv file path or a list.")
 
-    normalized_data = _normalize_address(data)
+    normalized_data = _normalize_address(data, api_path=api_path)  # api_path を _normalize_address に渡す
     if export_file:
         with open(export_file, 'w', newline='', encoding='utf-8') as file:
             writer = csv.DictWriter(file, fieldnames=normalized_data[0].keys())
             writer.writeheader()
             writer.writerows(normalized_data)
 
     return normalized_data
@@ -72,29 +74,35 @@
     file_list = load_config("file_id")
     # try to get file_id
     try:
         return file_list[prefecture.capitalize()]
     except KeyError as exp:
         raise SystemExit(f"Unexpected Key Value: {prefecture}") from exp
 
-def update_progress_and_normalize(corp, index, total_lines, progress_interval):
+def update_progress_and_normalize(corp, index, total_lines, progress_interval, api_path=None):  # api_path 引数を追加
     if index % progress_interval == 0:
         current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         print(f"{current_time} - Processing progress: {int((index / total_lines) * 100)}% complete")
     addr = str(corp['prefecture_name']) + str(corp['city_name']) + str(corp['street_number'])
-    corp.update(normalize(addr, endpoint=load_api()))
+    if api_path:
+        corp.update(normalize(addr, endpoint=api_path))  # api_path がある場合、endpoint として渡す
+    else:
+        corp.update(normalize(addr))
     return corp
 
-def _normalize_address(lines):
+def _normalize_address(lines, api_path=None):  # api_path 引数を追加
     total_lines = len(lines)
     print(f"Processing {total_lines} records.")
     progress_interval = total_lines // 10
 
     # functools.partialを使用して、追加の引数を設定
-    func = partial(update_progress_and_normalize, total_lines=total_lines, progress_interval=progress_interval)
+    if api_path:
+        func = partial(update_progress_and_normalize, total_lines=total_lines, progress_interval=progress_interval, api_path=api_path)
+    else:
+        func = partial(update_progress_and_normalize, total_lines=total_lines, progress_interval=progress_interval)
 
     with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
         # executor.mapに渡すために、funcを使用
         lines = list(executor.map(func, lines, range(total_lines)))
     current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     print(f"{current_time} - Processing progress: 100% complete")
```

### Comparing `cnparser-1.4.5/cnparser/utility.py` & `cnparser-1.4.6/cnparser/utility.py`

 * *Files identical despite different names*

### Comparing `cnparser-1.4.5/cnparser.egg-info/PKG-INFO` & `cnparser-1.4.6/cnparser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnparser
-Version: 1.4.5
+Version: 1.4.6
 Summary: cnparser is a parser library of Corporate Number Publication Site data.
 Home-page: https://github.com/new-village/cnparser
 Author: new-village
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -61,7 +61,19 @@
 
 #### Enrich information to CSV file  
 You can export enriched data to CSV file directry by `export_file` option with file name.
 ```python
 >>> import cnparser
 >>> enriched = cnparser.bulk_enrich(cndata, export_file="path/to/export/data.csv")
 ```
+
+#### Enrich information to CSV file with downloaded api
+If you enrich massive data, You can use downloaded api.
+```
+$ cd /home/<USER>/
+$ curl -sL https://github.com/geolonia/japanese-addresses/archive/refs/heads/master.tar.gz | tar xvfz -
+```
+  
+```python
+>>> import cnparser
+>>> enriched = cnparser.bulk_enrich(cndata, api_path="file:///home/<USER>/japanese-addresses-master/api/ja")
+```
```

### Comparing `cnparser-1.4.5/setup.py` & `cnparser-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='cnparser',
-    version='1.4.5',
+    version='1.4.6',
     author='new-village',
     url='https://github.com/new-village/cnparser',
     description='cnparser is a parser library of Corporate Number Publication Site data.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license = 'Apache License 2.0',
     install_requires=['requests', 'bs4', 'kanjize==1.5.0', 'normalize-japanese-addresses==0.0.9'],
```

### Comparing `cnparser-1.4.5/test/test_load.py` & `cnparser-1.4.6/test/test_load.py`

 * *Files identical despite different names*

