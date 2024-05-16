# Comparing `tmp/llama_index_multi_modal_llms_gemini-0.1.4.tar.gz` & `tmp/llama_index_multi_modal_llms_gemini-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_multi_modal_llms_gemini-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_multi_modal_llms_gemini-0.1.5.tar", max compression
```

## Comparing `llama_index_multi_modal_llms_gemini-0.1.4.tar` & `llama_index_multi_modal_llms_gemini-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       50 2024-03-20 20:45:24.847482 llama_index_multi_modal_llms_gemini-0.1.4/README.md
--rw-r--r--   0        0        0      102 2024-03-20 20:45:24.847482 llama_index_multi_modal_llms_gemini-0.1.4/llama_index/multi_modal_llms/gemini/__init__.py
--rw-r--r--   0        0        0     9169 2024-03-20 20:45:24.847482 llama_index_multi_modal_llms_gemini-0.1.4/llama_index/multi_modal_llms/gemini/base.py
--rw-r--r--   0        0        0     1557 2024-03-20 20:45:24.847482 llama_index_multi_modal_llms_gemini-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 llama_index_multi_modal_llms_gemini-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2024-04-08 18:10:06.507359 llama_index_multi_modal_llms_gemini-0.1.5/README.md
+-rw-r--r--   0        0        0      102 2024-04-08 18:10:06.507359 llama_index_multi_modal_llms_gemini-0.1.5/llama_index/multi_modal_llms/gemini/__init__.py
+-rw-r--r--   0        0        0     9169 2024-04-08 18:10:06.507359 llama_index_multi_modal_llms_gemini-0.1.5/llama_index/multi_modal_llms/gemini/base.py
+-rw-r--r--   0        0        0     1557 2024-04-08 18:10:06.507359 llama_index_multi_modal_llms_gemini-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      775 1970-01-01 00:00:00.000000 llama_index_multi_modal_llms_gemini-0.1.5/PKG-INFO
```

### Comparing `llama_index_multi_modal_llms_gemini-0.1.4/llama_index/multi_modal_llms/gemini/base.py` & `llama_index_multi_modal_llms_gemini-0.1.5/llama_index/multi_modal_llms/gemini/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_multi_modal_llms_gemini-0.1.4/pyproject.toml` & `llama_index_multi_modal_llms_gemini-0.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index multi-modal-llms gemini integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-multi-modal-llms-gemini"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.11.post1"
-llama-index-llms-gemini = "^0.1.1"
+llama-index-llms-gemini = "^0.1.7"
 pillow = "^10.2.0"
-google-generativeai = "^0.3.2"
+google-generativeai = "^0.4.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_multi_modal_llms_gemini-0.1.4/PKG-INFO` & `llama_index_multi_modal_llms_gemini-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-multi-modal-llms-gemini
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index multi-modal-llms gemini integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
+Requires-Dist: google-generativeai (>=0.4.1,<0.5.0)
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
-Requires-Dist: llama-index-llms-gemini (>=0.1.1,<0.2.0)
+Requires-Dist: llama-index-llms-gemini (>=0.1.7,<0.2.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Multi-Modal-Llms Integration: Gemini
```

