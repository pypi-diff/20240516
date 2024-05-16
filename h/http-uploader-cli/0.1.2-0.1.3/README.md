# Comparing `tmp/http_uploader_cli-0.1.2.tar.gz` & `tmp/http_uploader_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_uploader_cli-0.1.2.tar", max compression
+gzip compressed data, was "http_uploader_cli-0.1.3.tar", max compression
```

## Comparing `http_uploader_cli-0.1.2.tar` & `http_uploader_cli-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      157 2024-05-15 19:48:12.119711 http_uploader_cli-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-14 14:24:59.626808 http_uploader_cli-0.1.2/http_uploader/__init__.py
--rw-r--r--   0        0        0      808 2024-05-15 19:14:10.429257 http_uploader_cli-0.1.2/http_uploader/__main__.py
--rw-r--r--   0        0        0        0 2024-05-15 01:19:07.532409 http_uploader_cli-0.1.2/http_uploader/cli/__init__.py
--rw-r--r--   0        0        0      133 2024-05-15 18:29:20.585359 http_uploader_cli-0.1.2/http_uploader/cli/engine/__init__.py
--rw-r--r--   0        0        0      167 2024-05-15 18:27:39.210674 http_uploader_cli-0.1.2/http_uploader/cli/engine/common.py
--rw-r--r--   0        0        0        0 2024-05-15 02:56:37.081111 http_uploader_cli-0.1.2/http_uploader/cli/engine/dto/__init__.py
--rw-r--r--   0        0        0       62 2024-05-15 18:27:52.854638 http_uploader_cli-0.1.2/http_uploader/cli/engine/dto/args/__init__.py
--rw-r--r--   0        0        0      223 2024-05-15 18:27:06.039141 http_uploader_cli-0.1.2/http_uploader/cli/engine/dto/args/common.py
--rw-r--r--   0        0        0       60 2024-05-15 03:03:35.236855 http_uploader_cli-0.1.2/http_uploader/cli/engine/dto/response/__init__.py
--rw-r--r--   0        0        0      127 2024-05-15 18:00:46.836071 http_uploader_cli-0.1.2/http_uploader/cli/engine/dto/response/common.py
--rw-r--r--   0        0        0     1663 2024-05-15 19:15:35.236484 http_uploader_cli-0.1.2/http_uploader/cli/engine/http_uploader.py
--rw-r--r--   0        0        0        0 2024-05-15 03:03:20.402845 http_uploader_cli-0.1.2/http_uploader/facade/__init__.py
--rw-r--r--   0        0        0      169 2024-05-15 03:04:00.654680 http_uploader_cli-0.1.2/http_uploader/facade/common.py
--rw-r--r--   0        0        0     4096 2024-05-15 20:18:31.510181 http_uploader_cli-0.1.2/http_uploader/facade/http_uploader.py
--rw-r--r--   0        0        0      356 2024-05-15 14:30:36.910704 http_uploader_cli-0.1.2/http_uploader/facade/proxy.py
--rw-r--r--   0        0        0       92 2024-05-15 03:12:56.629106 http_uploader_cli-0.1.2/http_uploader/finder/__init__.py
--rw-r--r--   0        0        0      161 2024-05-15 18:44:31.720768 http_uploader_cli-0.1.2/http_uploader/finder/common.py
--rw-r--r--   0        0        0     1168 2024-05-15 18:45:32.296898 http_uploader_cli-0.1.2/http_uploader/finder/json.py
--rw-r--r--   0        0        0      108 2024-05-15 03:09:45.380393 http_uploader_cli-0.1.2/http_uploader/http/__init__.py
--rw-r--r--   0        0        0      197 2024-05-14 18:10:43.034518 http_uploader_cli-0.1.2/http_uploader/http/common.py
--rw-r--r--   0        0        0        0 2024-05-14 18:09:03.656460 http_uploader_cli-0.1.2/http_uploader/http/dto/__init__.py
--rw-r--r--   0        0        0      322 2024-05-15 18:15:43.114231 http_uploader_cli-0.1.2/http_uploader/http/dto/client_request.py
--rw-r--r--   0        0        0      110 2024-05-14 18:10:25.287008 http_uploader_cli-0.1.2/http_uploader/http/dto/response.py
--rw-r--r--   0        0        0      703 2024-05-15 14:30:36.910704 http_uploader_cli-0.1.2/http_uploader/http/post.py
--rw-r--r--   0        0        0        0 2024-05-14 15:11:39.866758 http_uploader_cli-0.1.2/http_uploader/utils/__init__.py
--rw-r--r--   0        0        0       97 2024-05-15 03:07:48.478399 http_uploader_cli-0.1.2/http_uploader/utils/file/__init__.py
--rw-r--r--   0        0        0      304 2024-05-15 18:20:54.025277 http_uploader_cli-0.1.2/http_uploader/utils/file/common.py
--rw-r--r--   0        0        0     1216 2024-05-15 19:25:06.249374 http_uploader_cli-0.1.2/http_uploader/utils/file/txt.py
--rw-r--r--   0        0        0      263 2024-05-15 18:48:33.058576 http_uploader_cli-0.1.2/http_uploader/utils/filter/__init__.py
--rw-r--r--   0        0        0      172 2024-05-15 02:43:18.401218 http_uploader_cli-0.1.2/http_uploader/utils/filter/common.py
--rw-r--r--   0        0        0      603 2024-05-15 02:37:58.119623 http_uploader_cli-0.1.2/http_uploader/utils/filter/compare.py
--rw-r--r--   0        0        0     1057 2024-05-15 02:37:59.573025 http_uploader_cli-0.1.2/http_uploader/utils/filter/extented_compare.py
--rw-r--r--   0        0        0      307 2024-05-15 19:38:01.824988 http_uploader_cli-0.1.2/http_uploader/utils/parts.py
--rw-r--r--   0        0        0     1524 2024-05-15 20:18:43.640740 http_uploader_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 http_uploader_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      157 2024-05-15 19:48:12.119711 http_uploader_cli-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-14 14:24:59.626808 http_uploader_cli-0.1.3/http_uploader/__init__.py
+-rw-r--r--   0        0        0      808 2024-05-15 19:14:10.429257 http_uploader_cli-0.1.3/http_uploader/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-15 01:19:07.532409 http_uploader_cli-0.1.3/http_uploader/cli/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-15 18:29:20.585359 http_uploader_cli-0.1.3/http_uploader/cli/engine/__init__.py
+-rw-r--r--   0        0        0      167 2024-05-15 18:27:39.210674 http_uploader_cli-0.1.3/http_uploader/cli/engine/common.py
+-rw-r--r--   0        0        0        0 2024-05-15 02:56:37.081111 http_uploader_cli-0.1.3/http_uploader/cli/engine/dto/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-15 18:27:52.854638 http_uploader_cli-0.1.3/http_uploader/cli/engine/dto/args/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-15 18:27:06.039141 http_uploader_cli-0.1.3/http_uploader/cli/engine/dto/args/common.py
+-rw-r--r--   0        0        0       60 2024-05-15 03:03:35.236855 http_uploader_cli-0.1.3/http_uploader/cli/engine/dto/response/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-15 18:00:46.836071 http_uploader_cli-0.1.3/http_uploader/cli/engine/dto/response/common.py
+-rw-r--r--   0        0        0     1663 2024-05-15 19:15:35.236484 http_uploader_cli-0.1.3/http_uploader/cli/engine/http_uploader.py
+-rw-r--r--   0        0        0        0 2024-05-15 03:03:20.402845 http_uploader_cli-0.1.3/http_uploader/facade/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-15 03:04:00.654680 http_uploader_cli-0.1.3/http_uploader/facade/common.py
+-rw-r--r--   0        0        0     4099 2024-05-15 20:27:40.642335 http_uploader_cli-0.1.3/http_uploader/facade/http_uploader.py
+-rw-r--r--   0        0        0      356 2024-05-15 14:30:36.910704 http_uploader_cli-0.1.3/http_uploader/facade/proxy.py
+-rw-r--r--   0        0        0       92 2024-05-15 03:12:56.629106 http_uploader_cli-0.1.3/http_uploader/finder/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-15 18:44:31.720768 http_uploader_cli-0.1.3/http_uploader/finder/common.py
+-rw-r--r--   0        0        0     1168 2024-05-15 20:24:53.541233 http_uploader_cli-0.1.3/http_uploader/finder/json.py
+-rw-r--r--   0        0        0      108 2024-05-15 03:09:45.380393 http_uploader_cli-0.1.3/http_uploader/http/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-14 18:10:43.034518 http_uploader_cli-0.1.3/http_uploader/http/common.py
+-rw-r--r--   0        0        0        0 2024-05-14 18:09:03.656460 http_uploader_cli-0.1.3/http_uploader/http/dto/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-15 18:15:43.114231 http_uploader_cli-0.1.3/http_uploader/http/dto/client_request.py
+-rw-r--r--   0        0        0      110 2024-05-14 18:10:25.287008 http_uploader_cli-0.1.3/http_uploader/http/dto/response.py
+-rw-r--r--   0        0        0      703 2024-05-15 14:30:36.910704 http_uploader_cli-0.1.3/http_uploader/http/post.py
+-rw-r--r--   0        0        0        0 2024-05-14 15:11:39.866758 http_uploader_cli-0.1.3/http_uploader/utils/__init__.py
+-rw-r--r--   0        0        0       97 2024-05-15 03:07:48.478399 http_uploader_cli-0.1.3/http_uploader/utils/file/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-15 18:20:54.025277 http_uploader_cli-0.1.3/http_uploader/utils/file/common.py
+-rw-r--r--   0        0        0     1216 2024-05-15 19:25:06.249374 http_uploader_cli-0.1.3/http_uploader/utils/file/txt.py
+-rw-r--r--   0        0        0      263 2024-05-15 18:48:33.058576 http_uploader_cli-0.1.3/http_uploader/utils/filter/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-15 02:43:18.401218 http_uploader_cli-0.1.3/http_uploader/utils/filter/common.py
+-rw-r--r--   0        0        0      603 2024-05-15 02:37:58.119623 http_uploader_cli-0.1.3/http_uploader/utils/filter/compare.py
+-rw-r--r--   0        0        0     1057 2024-05-15 02:37:59.573025 http_uploader_cli-0.1.3/http_uploader/utils/filter/extented_compare.py
+-rw-r--r--   0        0        0      307 2024-05-15 19:38:01.824988 http_uploader_cli-0.1.3/http_uploader/utils/parts.py
+-rw-r--r--   0        0        0     1524 2024-05-15 20:28:56.572531 http_uploader_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      847 1970-01-01 00:00:00.000000 http_uploader_cli-0.1.3/PKG-INFO
```

### Comparing `http_uploader_cli-0.1.2/http_uploader/__main__.py` & `http_uploader_cli-0.1.3/http_uploader/__main__.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.2/http_uploader/cli/engine/http_uploader.py` & `http_uploader_cli-0.1.3/http_uploader/cli/engine/http_uploader.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.2/http_uploader/facade/http_uploader.py` & `http_uploader_cli-0.1.3/http_uploader/facade/http_uploader.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,16 @@
     readed_strings = await file_reader.read(*positions_range)
     if cli_args.filter:
         result = []
         for json_string in readed_strings:
             filter_operands = cli_args.filter.split()
             json_object = json.loads(json_string)
             found_value = JsonFinder.from_json(json_object).search(filter_operands[0])
-            filtering_value = filter_operands[-1].strip("'\"")
-            if not found_value:
+            filtering_value = json.loads(filter_operands[-1])
+            if found_value is None:
                 continue
             if create_extented_compare_filter(filter_operands[1], found_value).check(  # type: ignore[arg-type]
                 filtering_value,
             ):
                 result.append(json_object)
     else:
         result = readed_strings
```

### Comparing `http_uploader_cli-0.1.2/http_uploader/finder/json.py` & `http_uploader_cli-0.1.3/http_uploader/finder/json.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.2/http_uploader/http/post.py` & `http_uploader_cli-0.1.3/http_uploader/http/post.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.2/http_uploader/utils/file/txt.py` & `http_uploader_cli-0.1.3/http_uploader/utils/file/txt.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.2/http_uploader/utils/filter/compare.py` & `http_uploader_cli-0.1.3/http_uploader/utils/filter/compare.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.2/http_uploader/utils/filter/extented_compare.py` & `http_uploader_cli-0.1.3/http_uploader/utils/filter/extented_compare.py`

 * *Files identical despite different names*

### Comparing `http_uploader_cli-0.1.2/pyproject.toml` & `http_uploader_cli-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "http-uploader-cli"
-version = "0.1.2"
+version = "0.1.3"
 description = "Simple HTTP CLI json data uploader"
 repository = "https://github.com/rafailmdzdv/http-uploader-cli"
 authors = ["rafailmdzdv <rafayt323@xmail.ru>"]
 readme = "README.md"
 packages = [ {include = "http_uploader"} ]
 
 [tool.poetry.dependencies]
```

### Comparing `http_uploader_cli-0.1.2/PKG-INFO` & `http_uploader_cli-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http-uploader-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple HTTP CLI json data uploader
 Home-page: https://github.com/rafailmdzdv/http-uploader-cli
 Author: rafailmdzdv
 Author-email: rafayt323@xmail.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

