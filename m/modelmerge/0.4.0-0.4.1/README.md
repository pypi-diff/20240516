# Comparing `tmp/modelmerge-0.4.0.tar.gz` & `tmp/modelmerge-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.4.0.tar", last modified: Tue May 14 13:49:04 2024, max compression
+gzip compressed data, was "modelmerge-0.4.1.tar", last modified: Thu May 16 05:44:19 2024, max compression
```

## Comparing `modelmerge-0.4.0.tar` & `modelmerge-0.4.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:49:04.352346 modelmerge-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-14 13:48:52.000000 modelmerge-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 13:49:04.352346 modelmerge-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-14 13:48:52.000000 modelmerge-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:49:04.352346 modelmerge-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-14 13:48:52.000000 modelmerge-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:49:04.344346 modelmerge-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:49:04.344346 modelmerge-0.4.0/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:49:04.344346 modelmerge-0.4.0/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30966 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:49:04.348346 modelmerge-0.4.0/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:49:04.348346 modelmerge-0.4.0/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:49:04.348346 modelmerge-0.4.0/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-14 13:48:52.000000 modelmerge-0.4.0/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:49:04.352346 modelmerge-0.4.0/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-14 13:49:04.000000 modelmerge-0.4.0/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-14 13:49:04.000000 modelmerge-0.4.0/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:49:04.000000 modelmerge-0.4.0/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-14 13:49:04.000000 modelmerge-0.4.0/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 13:49:04.000000 modelmerge-0.4.0/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:49:04.352346 modelmerge-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-14 13:48:52.000000 modelmerge-0.4.0/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:19.029546 modelmerge-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-16 05:44:09.000000 modelmerge-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-16 05:44:19.029546 modelmerge-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-16 05:44:09.000000 modelmerge-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:44:19.029546 modelmerge-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-16 05:44:09.000000 modelmerge-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:19.021546 modelmerge-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:19.021546 modelmerge-0.4.1/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:19.025546 modelmerge-0.4.1/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30966 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:19.025546 modelmerge-0.4.1/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:19.025546 modelmerge-0.4.1/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:19.025546 modelmerge-0.4.1/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-16 05:44:09.000000 modelmerge-0.4.1/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:19.029546 modelmerge-0.4.1/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-16 05:44:18.000000 modelmerge-0.4.1/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-16 05:44:18.000000 modelmerge-0.4.1/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:44:18.000000 modelmerge-0.4.1/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 05:44:18.000000 modelmerge-0.4.1/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 05:44:18.000000 modelmerge-0.4.1/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:44:19.029546 modelmerge-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 05:44:09.000000 modelmerge-0.4.1/test/test_whisper.py
```

### Comparing `modelmerge-0.4.0/LICENSE` & `modelmerge-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/PKG-INFO` & `modelmerge-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.0
+Version: 0.4.1
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.0/README.md` & `modelmerge-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.4.1/src/ModelMerge/models/chatgpt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/ModelMerge/models/claude.py` & `modelmerge-0.4.1/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/ModelMerge/models/config.py` & `modelmerge-0.4.1/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/ModelMerge/models/genimi.py` & `modelmerge-0.4.1/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/ModelMerge/models/groq.py` & `modelmerge-0.4.1/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.4.1/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.4.1/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/ModelMerge/tools/function_call.py` & `modelmerge-0.4.1/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/ModelMerge/utils/prompt.py` & `modelmerge-0.4.1/src/ModelMerge/utils/prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,24 +73,24 @@
     "周海媚"
     "周海媚 事件"
     "Kathy Chau Hoi Mei news"
     "这是我的问题：{source}"
 )
 
 system_prompt = (
-    "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally in {}. Knowledge cutoff: 2023-12. Current date: [ {} ]"
+    "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally in {}. Use simple characters to represent mathematical symbols. Do not use LaTeX commands. Knowledge cutoff: 2023-12. Current date: [ {} ]"
     # "Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about my question step by step and then answer my question based on the Search results provided. Please response with a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks."
 )
 
 chatgpt_system_prompt = (
-    "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally"
+    "You are ChatGPT, a large language model trained by OpenAI. Use simple characters to represent mathematical symbols. Do not use LaTeX commands. Respond conversationally"
 )
 
 claude_system_prompt = (
-    "You are Claude, a large language model trained by Anthropic. Respond conversationally in {}."
+    "You are Claude, a large language model trained by Anthropic. Use simple characters to represent mathematical symbols. Do not use LaTeX commands. Respond conversationally in {}."
 )
 
 search_system_prompt = (
     "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally in {}."
     "You can break down the task into multiple steps and search the web to answer my questions one by one."
     "you needs to follow the following strategies:"
     "- First, you need to analyze how many steps are required to answer my question.\n"
```

### Comparing `modelmerge-0.4.0/src/ModelMerge/utils/scripts.py` & `modelmerge-0.4.1/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.4.1/src/modelmerge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.0
+Version: 0.4.1
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.0/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.4.1/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_Web_crawler.py` & `modelmerge-0.4.1/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_claude_zh_char.py` & `modelmerge-0.4.1/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_ddg_search.py` & `modelmerge-0.4.1/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_download_pdf.py` & `modelmerge-0.4.1/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_google_search.py` & `modelmerge-0.4.1/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_jieba.py` & `modelmerge-0.4.1/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_json.py` & `modelmerge-0.4.1/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_langchain_search_old.py` & `modelmerge-0.4.1/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_logging.py` & `modelmerge-0.4.1/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_ollama.py` & `modelmerge-0.4.1/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_tikitoken.py` & `modelmerge-0.4.1/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_token.py` & `modelmerge-0.4.1/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.0/test/test_url.py` & `modelmerge-0.4.1/test/test_url.py`

 * *Files identical despite different names*

