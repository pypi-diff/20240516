# Comparing `tmp/langchain_xiao-0.0.2.tar.gz` & `tmp/langchain_xiao-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_xiao-0.0.2.tar", last modified: Wed May 15 09:06:48 2024, max compression
+gzip compressed data, was "langchain_xiao-0.0.3.tar", last modified: Wed May 15 09:34:14 2024, max compression
```

## Comparing `langchain_xiao-0.0.2.tar` & `langchain_xiao-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.515916 langchain_xiao-0.0.2/
--rw-rw-rw-   0        0        0     3237 2024-04-25 13:48:27.000000 langchain_xiao-0.0.2/.gitignore
--rw-rw-rw-   0        0        0     1087 2024-04-25 12:15:59.000000 langchain_xiao-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      949 2024-05-15 09:06:48.514916 langchain_xiao-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       87 2024-04-26 09:06:01.000000 langchain_xiao-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.456089 langchain_xiao-0.0.2/langchain_xiao/
--rw-rw-rw-   0        0        0       23 2024-05-15 09:04:17.000000 langchain_xiao-0.0.2/langchain_xiao/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.484123 langchain_xiao-0.0.2/langchain_xiao/chat_models/
--rw-rw-rw-   0        0        0      102 2024-05-15 09:01:59.000000 langchain_xiao-0.0.2/langchain_xiao/chat_models/__init__.py
--rw-rw-rw-   0        0        0      755 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/chat_models/baichuan.py
--rw-rw-rw-   0        0        0    14067 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/chat_models/llamacpp.py
--rw-rw-rw-   0        0        0     1235 2024-05-15 09:01:26.000000 langchain_xiao-0.0.2/langchain_xiao/chat_models/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.491734 langchain_xiao-0.0.2/langchain_xiao/embeddings/
--rw-rw-rw-   0        0        0       40 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/embeddings/__init__.py
--rw-rw-rw-   0        0        0     2376 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/embeddings/fastllm.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.499733 langchain_xiao-0.0.2/langchain_xiao/llms/
--rw-rw-rw-   0        0        0       32 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/llms/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/llms/gpt4all.py
--rw-rw-rw-   0        0        0     1115 2024-04-26 08:50:58.000000 langchain_xiao-0.0.2/langchain_xiao/llms/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.500733 langchain_xiao-0.0.2/langchain_xiao/retrievers/
--rw-rw-rw-   0        0        0        0 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/retrievers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.508917 langchain_xiao-0.0.2/langchain_xiao/retrievers/document_compressors/
--rw-rw-rw-   0        0        0       45 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/retrievers/document_compressors/__init__.py
--rw-rw-rw-   0        0        0     3212 2024-04-26 08:47:54.000000 langchain_xiao-0.0.2/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py
-drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.513917 langchain_xiao-0.0.2/langchain_xiao.egg-info/
--rw-rw-rw-   0        0        0      949 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      857 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-15 09:06:48.000000 langchain_xiao-0.0.2/langchain_xiao.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2024-04-26 08:56:51.000000 langchain_xiao-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       70 2024-04-25 13:09:39.000000 langchain_xiao-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 09:06:48.515916 langchain_xiao-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 09:06:48.512916 langchain_xiao-0.0.2/tests/
--rw-rw-rw-   0        0        0     1095 2024-05-15 09:05:12.000000 langchain_xiao-0.0.2/tests/chat_models_utils.py
--rw-rw-rw-   0        0        0      461 2024-04-26 08:50:58.000000 langchain_xiao-0.0.2/tests/fastllm_embeddings.py
--rw-rw-rw-   0        0        0      706 2024-04-26 08:50:58.000000 langchain_xiao-0.0.2/tests/fastllm_rerank.py
--rw-rw-rw-   0        0        0      495 2024-04-26 08:50:58.000000 langchain_xiao-0.0.2/tests/llms_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:34:14.350697 langchain_xiao-0.0.3/
+-rw-rw-rw-   0        0        0     3237 2024-04-25 13:48:27.000000 langchain_xiao-0.0.3/.gitignore
+-rw-rw-rw-   0        0        0     1087 2024-04-25 12:15:59.000000 langchain_xiao-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      949 2024-05-15 09:34:14.333670 langchain_xiao-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2024-04-26 09:06:01.000000 langchain_xiao-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 09:34:14.296019 langchain_xiao-0.0.3/langchain_xiao/
+-rw-rw-rw-   0        0        0       23 2024-05-15 09:34:05.000000 langchain_xiao-0.0.3/langchain_xiao/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:34:14.319020 langchain_xiao-0.0.3/langchain_xiao/chat_models/
+-rw-rw-rw-   0        0        0      102 2024-05-15 09:01:59.000000 langchain_xiao-0.0.3/langchain_xiao/chat_models/__init__.py
+-rw-rw-rw-   0        0        0      755 2024-04-26 08:47:54.000000 langchain_xiao-0.0.3/langchain_xiao/chat_models/baichuan.py
+-rw-rw-rw-   0        0        0     5307 2024-05-15 09:02:54.000000 langchain_xiao-0.0.3/langchain_xiao/chat_models/cyou.py
+-rw-rw-rw-   0        0        0    14067 2024-04-26 08:47:54.000000 langchain_xiao-0.0.3/langchain_xiao/chat_models/llamacpp.py
+-rw-rw-rw-   0        0        0     1235 2024-05-15 09:01:26.000000 langchain_xiao-0.0.3/langchain_xiao/chat_models/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:34:14.321044 langchain_xiao-0.0.3/langchain_xiao/embeddings/
+-rw-rw-rw-   0        0        0       40 2024-04-26 08:47:54.000000 langchain_xiao-0.0.3/langchain_xiao/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     2376 2024-04-26 08:47:54.000000 langchain_xiao-0.0.3/langchain_xiao/embeddings/fastllm.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:34:14.324020 langchain_xiao-0.0.3/langchain_xiao/llms/
+-rw-rw-rw-   0        0        0       32 2024-04-26 08:47:54.000000 langchain_xiao-0.0.3/langchain_xiao/llms/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-26 08:47:54.000000 langchain_xiao-0.0.3/langchain_xiao/llms/gpt4all.py
+-rw-rw-rw-   0        0        0     1115 2024-04-26 08:50:58.000000 langchain_xiao-0.0.3/langchain_xiao/llms/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:34:14.324675 langchain_xiao-0.0.3/langchain_xiao/retrievers/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:47:54.000000 langchain_xiao-0.0.3/langchain_xiao/retrievers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:34:14.326668 langchain_xiao-0.0.3/langchain_xiao/retrievers/document_compressors/
+-rw-rw-rw-   0        0        0       45 2024-04-26 08:47:54.000000 langchain_xiao-0.0.3/langchain_xiao/retrievers/document_compressors/__init__.py
+-rw-rw-rw-   0        0        0     3212 2024-04-26 08:47:54.000000 langchain_xiao-0.0.3/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py
+drwxrwxrwx   0        0        0        0 2024-05-15 09:34:14.332670 langchain_xiao-0.0.3/langchain_xiao.egg-info/
+-rw-rw-rw-   0        0        0      949 2024-05-15 09:34:14.000000 langchain_xiao-0.0.3/langchain_xiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      892 2024-05-15 09:34:14.000000 langchain_xiao-0.0.3/langchain_xiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 09:34:14.000000 langchain_xiao-0.0.3/langchain_xiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-15 09:34:14.000000 langchain_xiao-0.0.3/langchain_xiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-15 09:34:14.000000 langchain_xiao-0.0.3/langchain_xiao.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2024-04-26 08:56:51.000000 langchain_xiao-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       70 2024-04-25 13:09:39.000000 langchain_xiao-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 09:34:14.351669 langchain_xiao-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-15 09:34:14.331695 langchain_xiao-0.0.3/tests/
+-rw-rw-rw-   0        0        0     1095 2024-05-15 09:05:12.000000 langchain_xiao-0.0.3/tests/chat_models_utils.py
+-rw-rw-rw-   0        0        0      461 2024-04-26 08:50:58.000000 langchain_xiao-0.0.3/tests/fastllm_embeddings.py
+-rw-rw-rw-   0        0        0      706 2024-04-26 08:50:58.000000 langchain_xiao-0.0.3/tests/fastllm_rerank.py
+-rw-rw-rw-   0        0        0      495 2024-04-26 08:50:58.000000 langchain_xiao-0.0.3/tests/llms_utils.py
```

### Comparing `langchain_xiao-0.0.2/.gitignore` & `langchain_xiao-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/LICENSE` & `langchain_xiao-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/PKG-INFO` & `langchain_xiao-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-xiao
-Version: 0.0.2
+Version: 0.0.3
 Summary: langchain extension python package
 Author-email: xiaojinli <553555614@qq.com>
 License: MIT
 Project-URL: Documentation, https://github.com/xiaojinlii/langchain-xiao/blob/main/README.md
 Project-URL: Source, https://github.com/xiaojinlii/langchain-xiao
 Keywords: langchain
 Classifier: Programming Language :: Python :: 3
```

### Comparing `langchain_xiao-0.0.2/langchain_xiao/chat_models/baichuan.py` & `langchain_xiao-0.0.3/langchain_xiao/chat_models/baichuan.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/langchain_xiao/chat_models/llamacpp.py` & `langchain_xiao-0.0.3/langchain_xiao/chat_models/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/langchain_xiao/chat_models/utils.py` & `langchain_xiao-0.0.3/langchain_xiao/chat_models/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/langchain_xiao/embeddings/fastllm.py` & `langchain_xiao-0.0.3/langchain_xiao/embeddings/fastllm.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/langchain_xiao/llms/gpt4all.py` & `langchain_xiao-0.0.3/langchain_xiao/llms/gpt4all.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/langchain_xiao/llms/utils.py` & `langchain_xiao-0.0.3/langchain_xiao/llms/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py` & `langchain_xiao-0.0.3/langchain_xiao/retrievers/document_compressors/fastllm_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/langchain_xiao.egg-info/PKG-INFO` & `langchain_xiao-0.0.3/langchain_xiao.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-xiao
-Version: 0.0.2
+Version: 0.0.3
 Summary: langchain extension python package
 Author-email: xiaojinli <553555614@qq.com>
 License: MIT
 Project-URL: Documentation, https://github.com/xiaojinlii/langchain-xiao/blob/main/README.md
 Project-URL: Source, https://github.com/xiaojinlii/langchain-xiao
 Keywords: langchain
 Classifier: Programming Language :: Python :: 3
```

### Comparing `langchain_xiao-0.0.2/langchain_xiao.egg-info/SOURCES.txt` & `langchain_xiao-0.0.3/langchain_xiao.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 langchain_xiao.egg-info/PKG-INFO
 langchain_xiao.egg-info/SOURCES.txt
 langchain_xiao.egg-info/dependency_links.txt
 langchain_xiao.egg-info/requires.txt
 langchain_xiao.egg-info/top_level.txt
 langchain_xiao/chat_models/__init__.py
 langchain_xiao/chat_models/baichuan.py
+langchain_xiao/chat_models/cyou.py
 langchain_xiao/chat_models/llamacpp.py
 langchain_xiao/chat_models/utils.py
 langchain_xiao/embeddings/__init__.py
 langchain_xiao/embeddings/fastllm.py
 langchain_xiao/llms/__init__.py
 langchain_xiao/llms/gpt4all.py
 langchain_xiao/llms/utils.py
```

### Comparing `langchain_xiao-0.0.2/pyproject.toml` & `langchain_xiao-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/tests/chat_models_utils.py` & `langchain_xiao-0.0.3/tests/chat_models_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_xiao-0.0.2/tests/fastllm_rerank.py` & `langchain_xiao-0.0.3/tests/fastllm_rerank.py`

 * *Files identical despite different names*

