# Comparing `tmp/fastinference_llm-0.0.2.tar.gz` & `tmp/fastinference_llm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastinference_llm-0.0.2.tar", last modified: Wed May 15 07:33:19 2024, max compression
+gzip compressed data, was "fastinference_llm-0.0.4.tar", last modified: Thu May 16 07:41:36 2024, max compression
```

## Comparing `fastinference_llm-0.0.2.tar` & `fastinference_llm-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:33:19.239127 fastinference_llm-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 07:33:15.000000 fastinference_llm-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-15 07:33:19.239127 fastinference_llm-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-05-15 07:33:15.000000 fastinference_llm-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:33:19.239127 fastinference_llm-0.0.2/fastinference/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-15 07:33:15.000000 fastinference_llm-0.0.2/fastinference/FastInference.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-15 07:33:15.000000 fastinference_llm-0.0.2/fastinference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:33:19.239127 fastinference_llm-0.0.2/fastinference_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-05-15 07:33:19.000000 fastinference_llm-0.0.2/fastinference_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-15 07:33:19.000000 fastinference_llm-0.0.2/fastinference_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:33:19.000000 fastinference_llm-0.0.2/fastinference_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 07:33:19.000000 fastinference_llm-0.0.2/fastinference_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 07:33:19.000000 fastinference_llm-0.0.2/fastinference_llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-15 07:33:19.239127 fastinference_llm-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-15 07:33:15.000000 fastinference_llm-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:41:35.998925 fastinference_llm-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-05-16 07:41:35.998925 fastinference_llm-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10722 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:41:35.994925 fastinference_llm-0.0.4/fastinference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/FastInference.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:41:35.998925 fastinference_llm-0.0.4/fastinference/data_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/data_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/data_processing/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/data_processing/datablock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:41:35.998925 fastinference_llm-0.0.4/fastinference/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/managers/llm_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/managers/task_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:41:35.998925 fastinference_llm-0.0.4/fastinference/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/prompt/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:41:35.998925 fastinference_llm-0.0.4/fastinference/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/fastinference/utils/data_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:41:35.998925 fastinference_llm-0.0.4/fastinference_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-05-16 07:41:35.000000 fastinference_llm-0.0.4/fastinference_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-16 07:41:35.000000 fastinference_llm-0.0.4/fastinference_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:41:35.000000 fastinference_llm-0.0.4/fastinference_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 07:41:35.000000 fastinference_llm-0.0.4/fastinference_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 07:41:35.000000 fastinference_llm-0.0.4/fastinference_llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 07:41:35.998925 fastinference_llm-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-16 07:41:31.000000 fastinference_llm-0.0.4/setup.py
```

### Comparing `fastinference_llm-0.0.2/LICENSE.txt` & `fastinference_llm-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastinference_llm-0.0.2/PKG-INFO` & `fastinference_llm-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: fastinference-llm
-Version: 0.0.2
+Version: 0.0.4
 Summary: Seamlessly integrate with top LLM APIs for speedy, robust, and scalable querying. Ideal for developers needing quick, reliable AI-powered responses.
 Home-page: https://github.com/blefo/FastInference
-Download-URL: https://github.com/blefo/FastInference/archive/v_01.tar.gz
 Author: Baptiste Lefort
 Author-email: lefort.baptiste@icloud.com
 License: MIT
 Keywords: api,fast,inference,distributed,llm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: validators
-Requires-Dist: beautifulsoup4
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: backoff
+Requires-Dist: openai
+Requires-Dist: litellm
+Requires-Dist: tqdm
 
 <h1 align="center">
         ⚡FastInference - The Ultra-Fast LLM Querying Manager (OpenAi, HuggingFace, Ollama, ...)
 </h1>
 <p align="center">
             <p align="center">Query any LLM API and get the responses very fast with a <b> highly robust and distributed </b> library. <br>
             All the LLMs providers can be used with FastInference  [OpenAI, Huggingface, VertexAI, TogetherAI, Azure, etc.]
```

### Comparing `fastinference_llm-0.0.2/README.md` & `fastinference_llm-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fastinference_llm-0.0.2/fastinference/FastInference.py` & `fastinference_llm-0.0.4/fastinference/FastInference.py`

 * *Files identical despite different names*

### Comparing `fastinference_llm-0.0.2/fastinference_llm.egg-info/PKG-INFO` & `fastinference_llm-0.0.4/fastinference_llm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: fastinference-llm
-Version: 0.0.2
+Version: 0.0.4
 Summary: Seamlessly integrate with top LLM APIs for speedy, robust, and scalable querying. Ideal for developers needing quick, reliable AI-powered responses.
 Home-page: https://github.com/blefo/FastInference
-Download-URL: https://github.com/blefo/FastInference/archive/v_01.tar.gz
 Author: Baptiste Lefort
 Author-email: lefort.baptiste@icloud.com
 License: MIT
 Keywords: api,fast,inference,distributed,llm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: validators
-Requires-Dist: beautifulsoup4
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: backoff
+Requires-Dist: openai
+Requires-Dist: litellm
+Requires-Dist: tqdm
 
 <h1 align="center">
         ⚡FastInference - The Ultra-Fast LLM Querying Manager (OpenAi, HuggingFace, Ollama, ...)
 </h1>
 <p align="center">
             <p align="center">Query any LLM API and get the responses very fast with a <b> highly robust and distributed </b> library. <br>
             All the LLMs providers can be used with FastInference  [OpenAI, Huggingface, VertexAI, TogetherAI, Azure, etc.]
```

