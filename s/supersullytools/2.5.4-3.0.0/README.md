# Comparing `tmp/supersullytools-2.5.4.tar.gz` & `tmp/supersullytools-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supersullytools-2.5.4.tar", last modified: Wed May  8 16:54:12 2024, max compression
+gzip compressed data, was "supersullytools-3.0.0.tar", last modified: Thu May 16 20:53:37 2024, max compression
```

## Comparing `supersullytools-2.5.4.tar` & `supersullytools-3.0.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.679255 supersullytools-2.5.4/
--rw-r--r--   0 msull      (501) staff       (20)     1092 2023-11-08 05:22:30.000000 supersullytools-2.5.4/LICENSE
--rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-08 16:54:12.678480 supersullytools-2.5.4/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      297 2024-05-08 16:54:10.000000 supersullytools-2.5.4/README.md
--rw-r--r--   0 msull      (501) staff       (20)     2064 2024-05-08 16:54:10.000000 supersullytools-2.5.4/pyproject.toml
--rw-r--r--   0 msull      (501) staff       (20)       38 2024-05-08 16:54:12.679415 supersullytools-2.5.4/setup.cfg
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.660742 supersullytools-2.5.4/src/
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.662578 supersullytools-2.5.4/src/streamlit_app/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-30 16:56:26.000000 supersullytools-2.5.4/src/streamlit_app/Home.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.663352 supersullytools-2.5.4/src/streamlit_app/pages/
--rw-r--r--   0 msull      (501) staff       (20)     3497 2024-02-16 00:42:29.000000 supersullytools-2.5.4/src/streamlit_app/pages/AI Chat.py
--rw-r--r--   0 msull      (501) staff       (20)     1328 2024-02-15 00:27:25.000000 supersullytools-2.5.4/src/streamlit_app/pages/Item Paginator.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.663662 supersullytools-2.5.4/src/supersullytools/
--rw-r--r--   0 msull      (501) staff       (20)       26 2024-05-08 16:54:10.000000 supersullytools-2.5.4/src/supersullytools/__init__.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.666497 supersullytools-2.5.4/src/supersullytools/llm/
--rw-r--r--   0 msull      (501) staff       (20)        0 2024-05-06 20:11:38.000000 supersullytools-2.5.4/src/supersullytools/llm/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)    16767 2024-05-08 16:43:43.000000 supersullytools-2.5.4/src/supersullytools/llm/completions.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.667418 supersullytools-2.5.4/src/supersullytools/openai/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:46.000000 supersullytools-2.5.4/src/supersullytools/openai/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)     4329 2024-05-06 20:17:43.000000 supersullytools-2.5.4/src/supersullytools/openai/chat_session.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.669228 supersullytools-2.5.4/src/supersullytools/streamlit/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:34.000000 supersullytools-2.5.4/src/supersullytools/streamlit/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)      571 2024-03-21 19:38:09.000000 supersullytools-2.5.4/src/supersullytools/streamlit/misc.py
--rw-r--r--   0 msull      (501) staff       (20)     6115 2023-11-30 16:44:47.000000 supersullytools-2.5.4/src/supersullytools/streamlit/paginator.py
--rw-r--r--   0 msull      (501) staff       (20)    12742 2024-05-07 18:06:20.000000 supersullytools-2.5.4/src/supersullytools/streamlit/sessions.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.670351 supersullytools-2.5.4/src/supersullytools/utils/
--rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 18:02:43.000000 supersullytools-2.5.4/src/supersullytools/utils/__init__.py
--rw-r--r--   0 msull      (501) staff       (20)     7607 2024-05-06 23:02:18.000000 supersullytools-2.5.4/src/supersullytools/utils/fuzzy_search.py
--rw-r--r--   0 msull      (501) staff       (20)     1396 2024-02-15 22:47:53.000000 supersullytools-2.5.4/src/supersullytools/utils/misc.py
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.672388 supersullytools-2.5.4/src/supersullytools.egg-info/
--rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-08 16:54:12.000000 supersullytools-2.5.4/src/supersullytools.egg-info/PKG-INFO
--rw-r--r--   0 msull      (501) staff       (20)      906 2024-05-08 16:54:12.000000 supersullytools-2.5.4/src/supersullytools.egg-info/SOURCES.txt
--rw-r--r--   0 msull      (501) staff       (20)        1 2024-05-08 16:54:12.000000 supersullytools-2.5.4/src/supersullytools.egg-info/dependency_links.txt
--rw-r--r--   0 msull      (501) staff       (20)      289 2024-05-08 16:54:12.000000 supersullytools-2.5.4/src/supersullytools.egg-info/requires.txt
--rw-r--r--   0 msull      (501) staff       (20)       36 2024-05-08 16:54:12.000000 supersullytools-2.5.4/src/supersullytools.egg-info/top_level.txt
-drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-08 16:54:12.671687 supersullytools-2.5.4/src/tests/
--rw-r--r--   0 msull      (501) staff       (20)     5073 2024-05-06 20:18:38.000000 supersullytools-2.5.4/src/tests/conftest.py
--rw-r--r--   0 msull      (501) staff       (20)     4082 2024-05-06 22:59:37.000000 supersullytools-2.5.4/src/tests/test_fuzzy_search.py
--rw-r--r--   0 msull      (501) staff       (20)      795 2024-02-16 00:44:38.000000 supersullytools-2.5.4/src/tests/test_streamlit_session.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.599308 supersullytools-3.0.0/
+-rw-r--r--   0 msull      (501) staff       (20)     1092 2023-11-08 05:22:30.000000 supersullytools-3.0.0/LICENSE
+-rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-16 20:53:37.598875 supersullytools-3.0.0/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      297 2024-05-16 20:53:34.000000 supersullytools-3.0.0/README.md
+-rw-r--r--   0 msull      (501) staff       (20)     2064 2024-05-16 20:53:34.000000 supersullytools-3.0.0/pyproject.toml
+-rw-r--r--   0 msull      (501) staff       (20)       38 2024-05-16 20:53:37.599392 supersullytools-3.0.0/setup.cfg
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.586633 supersullytools-3.0.0/src/
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.587973 supersullytools-3.0.0/src/streamlit_app/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-30 16:56:26.000000 supersullytools-3.0.0/src/streamlit_app/Home.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.588653 supersullytools-3.0.0/src/streamlit_app/pages/
+-rw-r--r--   0 msull      (501) staff       (20)     3497 2024-02-16 00:42:29.000000 supersullytools-3.0.0/src/streamlit_app/pages/AI Chat.py
+-rw-r--r--   0 msull      (501) staff       (20)     1328 2024-02-15 00:27:25.000000 supersullytools-3.0.0/src/streamlit_app/pages/Item Paginator.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.588950 supersullytools-3.0.0/src/supersullytools/
+-rw-r--r--   0 msull      (501) staff       (20)       26 2024-05-16 20:53:34.000000 supersullytools-3.0.0/src/supersullytools/__init__.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.591741 supersullytools-3.0.0/src/supersullytools/llm/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2024-05-06 20:11:38.000000 supersullytools-3.0.0/src/supersullytools/llm/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)    16950 2024-05-16 20:50:33.000000 supersullytools-3.0.0/src/supersullytools/llm/completions.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.592357 supersullytools-3.0.0/src/supersullytools/openai/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:46.000000 supersullytools-3.0.0/src/supersullytools/openai/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)     4329 2024-05-06 20:17:43.000000 supersullytools-3.0.0/src/supersullytools/openai/chat_session.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.593509 supersullytools-3.0.0/src/supersullytools/streamlit/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 06:06:34.000000 supersullytools-3.0.0/src/supersullytools/streamlit/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)      571 2024-03-21 19:38:09.000000 supersullytools-3.0.0/src/supersullytools/streamlit/misc.py
+-rw-r--r--   0 msull      (501) staff       (20)     6115 2023-11-30 16:44:47.000000 supersullytools-3.0.0/src/supersullytools/streamlit/paginator.py
+-rw-r--r--   0 msull      (501) staff       (20)    12742 2024-05-07 18:06:20.000000 supersullytools-3.0.0/src/supersullytools/streamlit/sessions.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.594331 supersullytools-3.0.0/src/supersullytools/utils/
+-rw-r--r--   0 msull      (501) staff       (20)        0 2023-11-08 18:02:43.000000 supersullytools-3.0.0/src/supersullytools/utils/__init__.py
+-rw-r--r--   0 msull      (501) staff       (20)     7607 2024-05-06 23:02:18.000000 supersullytools-3.0.0/src/supersullytools/utils/fuzzy_search.py
+-rw-r--r--   0 msull      (501) staff       (20)     1396 2024-02-15 22:47:53.000000 supersullytools-3.0.0/src/supersullytools/utils/misc.py
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.595587 supersullytools-3.0.0/src/supersullytools.egg-info/
+-rw-r--r--   0 msull      (501) staff       (20)     3185 2024-05-16 20:53:37.000000 supersullytools-3.0.0/src/supersullytools.egg-info/PKG-INFO
+-rw-r--r--   0 msull      (501) staff       (20)      906 2024-05-16 20:53:37.000000 supersullytools-3.0.0/src/supersullytools.egg-info/SOURCES.txt
+-rw-r--r--   0 msull      (501) staff       (20)        1 2024-05-16 20:53:37.000000 supersullytools-3.0.0/src/supersullytools.egg-info/dependency_links.txt
+-rw-r--r--   0 msull      (501) staff       (20)      289 2024-05-16 20:53:37.000000 supersullytools-3.0.0/src/supersullytools.egg-info/requires.txt
+-rw-r--r--   0 msull      (501) staff       (20)       36 2024-05-16 20:53:37.000000 supersullytools-3.0.0/src/supersullytools.egg-info/top_level.txt
+drwxr-xr-x   0 msull      (501) staff       (20)        0 2024-05-16 20:53:37.595202 supersullytools-3.0.0/src/tests/
+-rw-r--r--   0 msull      (501) staff       (20)     5073 2024-05-06 20:18:38.000000 supersullytools-3.0.0/src/tests/conftest.py
+-rw-r--r--   0 msull      (501) staff       (20)     4082 2024-05-06 22:59:37.000000 supersullytools-3.0.0/src/tests/test_fuzzy_search.py
+-rw-r--r--   0 msull      (501) staff       (20)      795 2024-02-16 00:44:38.000000 supersullytools-3.0.0/src/tests/test_streamlit_session.py
```

### Comparing `supersullytools-2.5.4/LICENSE` & `supersullytools-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/PKG-INFO` & `supersullytools-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supersullytools
-Version: 2.5.4
+Version: 3.0.0
 Summary: This is a Python package that brings together a suite of utilities and helpers across several domains of software development.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -49,11 +49,11 @@
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 SuperSully Tools
 ================
 
-**Latest Version:** 2.5.4
+**Latest Version:** 3.0.0
 
 **SupersullyTools** is a Python package that brings together a suite of utilities and helpers across several domains of
 software development. My personal toolkit of things I want in every package I'm working on, compiled in one place.
```

### Comparing `supersullytools-2.5.4/pyproject.toml` & `supersullytools-3.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "supersullytools"
-version = "2.5.4"
+version = "3.0.0"
 description = "This is a Python package that brings together a suite of utilities and helpers across several domains of software development."
 readme = "README.md"
 authors = [{ name = "Sully", email = "sully@sadburger.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -62,15 +62,15 @@
 line-length = 120
 
 [tool.ruff]
 line-length = 120
 target-version = "py310"
 
 [tool.bumpver]
-current_version = "2.5.4"
+current_version = "3.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `supersullytools-2.5.4/src/streamlit_app/pages/AI Chat.py` & `supersullytools-3.0.0/src/streamlit_app/pages/AI Chat.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/streamlit_app/pages/Item Paginator.py` & `supersullytools-3.0.0/src/streamlit_app/pages/Item Paginator.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/supersullytools/llm/completions.py` & `supersullytools-3.0.0/src/supersullytools/llm/completions.py`

 * *Files 4% similar despite different names*

```diff
@@ -255,38 +255,38 @@
             output_tokens=openai_response.usage.completion_tokens,
             llm_metadata=CompletionModel.model_validate(llm, from_attributes=True),
             generated_at=finished_at,
             completion_time_ms=int((finished_at - started_at).total_seconds() * 1000),
         )
 
 
-class Gpt3p5Turbo0125(OpenAiModel):
+class Gpt3p5Turbo(OpenAiModel):
     make: str = "OpenAI"
     llm: str = "GPT 3.5 Turbo"
-    llm_id: str = "gpt-3.5-turbo-0125"
+    llm_id: str = "gpt-3.5-turbo"
     input_price_per_1k: float = 0.000500
     output_price_per_1k: float = 0.001500
     supports_images: bool = False
 
 
-class Gpt4Turbo0125Preview(Gpt3p5Turbo0125):
+class Gpt4Turbo(Gpt3p5Turbo):
     make: str = "OpenAI"
     llm: str = "GPT 4 Turbo"
-    llm_id: str = "gpt-4-0125-preview"
+    llm_id: str = "gpt-4-turbo"
     input_price_per_1k: float = 0.010000
     output_price_per_1k: float = 0.030000
-    supports_images: bool = False
+    supports_images: bool = True
 
 
-class Gpt4VisionPreview(Gpt3p5Turbo0125):
+class Gpt4Omni(Gpt3p5Turbo):
     make: str = "OpenAI"
-    llm: str = "GPT 4 Vision Preview"
-    llm_id: str = "gpt-4-vision-preview"
-    input_price_per_1k: float = 0.010000
-    output_price_per_1k: float = 0.030000
+    llm: str = "GPT 4 Omni"
+    llm_id: str = "gpt-4o"
+    input_price_per_1k: float = 0.005
+    output_price_per_1k: float = 0.015
     supports_images: bool = True
 
 
 class Llama2Chat13B(BedrockModel):
     make: str = "Meta"
     llm: str = "Llama 2 Chat 13B"
     llm_id: str = "meta.llama2-13b-chat-v1"
@@ -392,14 +392,23 @@
     llm: str = "Claude 3 Haiku"
     llm_id: str = "anthropic.claude-3-haiku-20240307-v1:0"
     input_price_per_1k: float = 0.00025
     output_price_per_1k: float = 0.00125
     supports_images: bool = True
 
 
+class Claude3Opus(Claude3Sonnet):
+    make: str = "Anthropic"
+    llm: str = "Claude 3 Opus"
+    llm_id: str = "anthropic.claude-3-opus-20240229-v1:0"
+    input_price_per_1k: float = 0.015
+    output_price_per_1k: float = 0.075
+    supports_images: bool = True
+
+
 class Mistral7B(BedrockModel):
     make: str = "Mistral AI"
     llm: str = "Mistral 7B Instruct"
     llm_id: str = "mistral.mistral-7b-instruct-v0:2"
     input_price_per_1k: float = 0.000150
     output_price_per_1k: float = 0.000200
     supports_images: bool = False
@@ -432,17 +441,18 @@
     llm_id: str = "mistral.mixtral-8x7b-instruct-v0:1"
     input_price_per_1k: float = 0.000450
     output_price_per_1k: float = 0.000700
     supports_images: bool = False
 
 
 ALL_MODELS = [
-    Gpt3p5Turbo0125(),
-    Gpt4Turbo0125Preview(),
-    Gpt4VisionPreview(),
+    Gpt3p5Turbo(),
+    Gpt4Omni(),
+    Gpt4Turbo(),
     Llama2Chat13B(),
     Llama2Chat70B(),
     Mistral7B(),
     Mixtral8x7B(),
     Claude3Haiku(),
     Claude3Sonnet(),
+    Claude3Opus(),
 ]
```

### Comparing `supersullytools-2.5.4/src/supersullytools/openai/chat_session.py` & `supersullytools-3.0.0/src/supersullytools/openai/chat_session.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/supersullytools/streamlit/misc.py` & `supersullytools-3.0.0/src/supersullytools/streamlit/misc.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/supersullytools/streamlit/paginator.py` & `supersullytools-3.0.0/src/supersullytools/streamlit/paginator.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/supersullytools/streamlit/sessions.py` & `supersullytools-3.0.0/src/supersullytools/streamlit/sessions.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/supersullytools/utils/fuzzy_search.py` & `supersullytools-3.0.0/src/supersullytools/utils/fuzzy_search.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/supersullytools/utils/misc.py` & `supersullytools-3.0.0/src/supersullytools/utils/misc.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/supersullytools.egg-info/PKG-INFO` & `supersullytools-3.0.0/src/supersullytools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supersullytools
-Version: 2.5.4
+Version: 3.0.0
 Summary: This is a Python package that brings together a suite of utilities and helpers across several domains of software development.
 Author-email: Sully <sully@sadburger.com>
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -49,11 +49,11 @@
 Provides-Extra: build
 Requires-Dist: build; extra == "build"
 Requires-Dist: twine; extra == "build"
 
 SuperSully Tools
 ================
 
-**Latest Version:** 2.5.4
+**Latest Version:** 3.0.0
 
 **SupersullyTools** is a Python package that brings together a suite of utilities and helpers across several domains of
 software development. My personal toolkit of things I want in every package I'm working on, compiled in one place.
```

### Comparing `supersullytools-2.5.4/src/supersullytools.egg-info/SOURCES.txt` & `supersullytools-3.0.0/src/supersullytools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/tests/conftest.py` & `supersullytools-3.0.0/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/tests/test_fuzzy_search.py` & `supersullytools-3.0.0/src/tests/test_fuzzy_search.py`

 * *Files identical despite different names*

### Comparing `supersullytools-2.5.4/src/tests/test_streamlit_session.py` & `supersullytools-3.0.0/src/tests/test_streamlit_session.py`

 * *Files identical despite different names*

