# Comparing `tmp/totokenizers-1.2.5.3.tar.gz` & `tmp/totokenizers-1.2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totokenizers-1.2.5.3.tar", last modified: Wed May 15 20:16:46 2024, max compression
+gzip compressed data, was "totokenizers-1.2.5.4.tar", last modified: Thu May 16 14:16:48 2024, max compression
```

## Comparing `totokenizers-1.2.5.3.tar` & `totokenizers-1.2.5.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:16:46.524119 totokenizers-1.2.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-15 20:16:46.524119 totokenizers-1.2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 20:16:46.524119 totokenizers-1.2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:16:46.520118 totokenizers-1.2.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/tests/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/tests/test_jsonschema_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/tests/test_openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:16:46.520118 totokenizers-1.2.5.3/totokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:16:46.524119 totokenizers-1.2.5.3/totokenizers/anthropic/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/anthropic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/anthropic/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/anthropic/info.py
--rw-r--r--   0 runner    (1001) docker     (127)  1774213 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/anthropic/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:16:46.524119 totokenizers-1.2.5.3/totokenizers/google/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/google/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/jsonschema_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:16:46.524119 totokenizers-1.2.5.3/totokenizers/mockai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/mockai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/mockai/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/mockai/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/model_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/openai_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-15 20:16:31.000000 totokenizers-1.2.5.3/totokenizers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 20:16:46.524119 totokenizers-1.2.5.3/totokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-15 20:16:46.000000 totokenizers-1.2.5.3/totokenizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-15 20:16:46.000000 totokenizers-1.2.5.3/totokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:16:46.000000 totokenizers-1.2.5.3/totokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 20:16:46.000000 totokenizers-1.2.5.3/totokenizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-15 20:16:46.000000 totokenizers-1.2.5.3/totokenizers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 20:16:46.000000 totokenizers-1.2.5.3/totokenizers.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:16:48.181382 totokenizers-1.2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-16 14:16:48.177382 totokenizers-1.2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:16:48.181382 totokenizers-1.2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:16:48.173382 totokenizers-1.2.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/tests/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/tests/test_jsonschema_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/tests/test_openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:16:48.173382 totokenizers-1.2.5.4/totokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:16:48.177382 totokenizers-1.2.5.4/totokenizers/anthropic/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/anthropic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/anthropic/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/anthropic/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1774213 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/anthropic/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:16:48.177382 totokenizers-1.2.5.4/totokenizers/google/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/google/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/jsonschema_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:16:48.177382 totokenizers-1.2.5.4/totokenizers/mockai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/mockai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/mockai/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/mockai/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/model_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/openai_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 14:16:38.000000 totokenizers-1.2.5.4/totokenizers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:16:48.177382 totokenizers-1.2.5.4/totokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-16 14:16:48.000000 totokenizers-1.2.5.4/totokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-16 14:16:48.000000 totokenizers-1.2.5.4/totokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:16:48.000000 totokenizers-1.2.5.4/totokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 14:16:48.000000 totokenizers-1.2.5.4/totokenizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 14:16:48.000000 totokenizers-1.2.5.4/totokenizers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:16:48.000000 totokenizers-1.2.5.4/totokenizers.egg-info/zip-safe
```

### Comparing `totokenizers-1.2.5.3/PKG-INFO` & `totokenizers-1.2.5.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totokenizers
-Version: 1.2.5.3
+Version: 1.2.5.4
 Summary: Text tokenizers.
 Home-page: https://github.com/TeiaLabs/totokenizers
 Author: TeiaLabs
 Author-email: contato@teialabs.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: google-cloud-aiplatform
```

### Comparing `totokenizers-1.2.5.3/README.md` & `totokenizers-1.2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/setup.py` & `totokenizers-1.2.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/tests/test_anthropic.py` & `totokenizers-1.2.5.4/tests/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/tests/test_code.py` & `totokenizers-1.2.5.4/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/tests/test_jsonschema_formatter.py` & `totokenizers-1.2.5.4/tests/test_jsonschema_formatter.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/tests/test_openai.py` & `totokenizers-1.2.5.4/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/anthropic/anthropic.py` & `totokenizers-1.2.5.4/totokenizers/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/anthropic/info.py` & `totokenizers-1.2.5.4/totokenizers/anthropic/info.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/anthropic/tokenizer.json` & `totokenizers-1.2.5.4/totokenizers/anthropic/tokenizer.json`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/errors.py` & `totokenizers-1.2.5.4/totokenizers/errors.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/factories.py` & `totokenizers-1.2.5.4/totokenizers/factories.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/google/google.py` & `totokenizers-1.2.5.4/totokenizers/google/google.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/jsonschema_formatter.py` & `totokenizers-1.2.5.4/totokenizers/jsonschema_formatter.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/mockai/info.py` & `totokenizers-1.2.5.4/totokenizers/mockai/info.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/mockai/tokenizer.py` & `totokenizers-1.2.5.4/totokenizers/mockai/tokenizer.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/model_info.py` & `totokenizers-1.2.5.4/totokenizers/model_info.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/openai.py` & `totokenizers-1.2.5.4/totokenizers/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,22 +59,23 @@
             "gpt-3.5-turbo-0613",
             "gpt-3.5-turbo-16k-0613",
             "gpt-4-0613",
             "gpt-4-32k-0613",
             "gpt-3.5-turbo-1106",
             "gpt-4-1106-preview",
             "gpt-4-0125-preview",
-            "gpt-4-turbo-preview", # currently points to gpt-4-0125-preview
+            "gpt-4-turbo-preview",  # currently points to gpt-4-0125-preview
             "gpt-4-32k-0314",
             "gpt-4-32k-0613",
             "gpt-4-turbo-2024-04-09",
             "gpt-3.5-turbo-0125",
             "gpt-4-turbo-2024-04-09",
             "gpt-4o-2024-05-13",
             "gpt-4o",
+            "gpt-3.5-turbo",
         }:
             self.tokens_per_message = 3
             self.tokens_per_name = 1
         elif self.model == "gpt-3.5-turbo-0301":
             self.tokens_per_message = (
                 4  # every message follows <|start|>{role/name}\n{content}<|end|>\n
             )
```

### Comparing `totokenizers-1.2.5.3/totokenizers/openai_info.py` & `totokenizers-1.2.5.4/totokenizers/openai_info.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/protocols.py` & `totokenizers-1.2.5.4/totokenizers/protocols.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers/schemas.py` & `totokenizers-1.2.5.4/totokenizers/schemas.py`

 * *Files identical despite different names*

### Comparing `totokenizers-1.2.5.3/totokenizers.egg-info/PKG-INFO` & `totokenizers-1.2.5.4/totokenizers.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totokenizers
-Version: 1.2.5.3
+Version: 1.2.5.4
 Summary: Text tokenizers.
 Home-page: https://github.com/TeiaLabs/totokenizers
 Author: TeiaLabs
 Author-email: contato@teialabs.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: google-cloud-aiplatform
```

### Comparing `totokenizers-1.2.5.3/totokenizers.egg-info/SOURCES.txt` & `totokenizers-1.2.5.4/totokenizers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

