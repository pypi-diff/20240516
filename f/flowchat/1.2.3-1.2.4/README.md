# Comparing `tmp/flowchat-1.2.3.tar.gz` & `tmp/flowchat-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchat-1.2.3.tar", last modified: Tue Apr 16 05:18:56 2024, max compression
+gzip compressed data, was "flowchat-1.2.4.tar", last modified: Thu May 16 17:28:13 2024, max compression
```

## Comparing `flowchat-1.2.3.tar` & `flowchat-1.2.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 05:18:56.615728 flowchat-1.2.3/
--rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.2.3/LICENSE
--rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 05:18:56.615492 flowchat-1.2.3/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.2.3/README.md
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 05:18:56.612342 flowchat-1.2.3/flowchat/
--rw-r--r--   0 flatypus   (501) staff       (20)       81 2024-04-16 03:29:58.000000 flowchat-1.2.3/flowchat/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.2.3/flowchat/autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)    11608 2024-04-16 05:18:16.000000 flowchat-1.2.3/flowchat/chain.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 05:18:56.613490 flowchat-1.2.3/flowchat/private/
--rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.2.3/flowchat/private/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)     5288 2024-04-16 05:14:01.000000 flowchat-1.2.3/flowchat/private/_private_helpers.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1470 2024-04-16 05:08:16.000000 flowchat-1.2.3/flowchat/types.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 05:18:56.615233 flowchat-1.2.3/flowchat.egg-info/
--rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 05:18:56.000000 flowchat-1.2.3/flowchat.egg-info/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)      455 2024-04-16 05:18:56.000000 flowchat-1.2.3/flowchat.egg-info/SOURCES.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-04-16 05:18:56.000000 flowchat-1.2.3/flowchat.egg-info/dependency_links.txt
--rw-r--r--   0 flatypus   (501) staff       (20)       32 2024-04-16 05:18:56.000000 flowchat-1.2.3/flowchat.egg-info/requires.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-04-16 05:18:56.000000 flowchat-1.2.3/flowchat.egg-info/top_level.txt
--rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.2.3/pyproject.toml
--rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-04-16 05:18:56.615779 flowchat-1.2.3/setup.cfg
--rw-r--r--   0 flatypus   (501) staff       (20)     1391 2024-04-16 05:18:45.000000 flowchat-1.2.3/setup.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 05:18:56.614903 flowchat-1.2.3/tests/
--rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.2.3/tests/test_autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4250 2024-04-16 02:44:31.000000 flowchat-1.2.3/tests/test_chaining.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.2.3/tests/test_config.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4765 2024-04-16 02:44:31.000000 flowchat-1.2.3/tests/test_pull.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.2.3/tests/test_stream.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.639593 flowchat-1.2.4/
+-rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.2.4/LICENSE
+-rw-r--r--   0 flatypus   (501) staff       (20)     7640 2024-05-16 17:28:13.639333 flowchat-1.2.4/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.2.4/README.md
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.635906 flowchat-1.2.4/flowchat/
+-rw-r--r--   0 flatypus   (501) staff       (20)       81 2024-04-16 03:29:58.000000 flowchat-1.2.4/flowchat/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.2.4/flowchat/autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)    11642 2024-05-16 17:25:48.000000 flowchat-1.2.4/flowchat/chain.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.637094 flowchat-1.2.4/flowchat/private/
+-rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.2.4/flowchat/private/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      752 2024-05-16 17:27:36.000000 flowchat-1.2.4/flowchat/private/_private_helpers.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     2098 2024-05-16 17:23:53.000000 flowchat-1.2.4/flowchat/types.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.638992 flowchat-1.2.4/flowchat.egg-info/
+-rw-r--r--   0 flatypus   (501) staff       (20)     7640 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)      455 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)       23 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/requires.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/top_level.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.2.4/pyproject.toml
+-rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-05-16 17:28:13.639639 flowchat-1.2.4/setup.cfg
+-rw-r--r--   0 flatypus   (501) staff       (20)     1379 2024-05-16 17:28:05.000000 flowchat-1.2.4/setup.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.638708 flowchat-1.2.4/tests/
+-rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.2.4/tests/test_autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4250 2024-04-16 02:44:31.000000 flowchat-1.2.4/tests/test_chaining.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.2.4/tests/test_config.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4765 2024-04-16 02:44:31.000000 flowchat-1.2.4/tests/test_pull.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.2.4/tests/test_stream.py
```

### Comparing `flowchat-1.2.3/LICENSE` & `flowchat-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.3/PKG-INFO` & `flowchat-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.2.3
+Version: 1.2.4
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: Pillow
-Requires-Dist: tiktoken
 Requires-Dist: requests
 
 # flowchat - clean, readable, logical code.
 
 [![PyPI version](https://img.shields.io/pypi/v/flowchat.svg)](https://pypi.org/project/flowchat/)
 [![License](https://img.shields.io/pypi/l/flowchat?logoColor=blue)](LICENSE.txt)
 ![Downloads](https://img.shields.io/pypi/dm/flowchat?logoColor=blue)
```

### Comparing `flowchat-1.2.3/README.md` & `flowchat-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.3/flowchat/autodedent.py` & `flowchat-1.2.4/flowchat/autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.3/flowchat/chain.py` & `flowchat-1.2.4/flowchat/chain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .autodedent import autodedent
-from .private._private_helpers import encode_image, CountStreamTokens
+from .private._private_helpers import encode_image, wrap_stream_and_count
 from .types import *
 from datetime import datetime
 from typing import List, Optional, Union, Callable, Any, Generator
 from typing_extensions import Unpack
 import json
 import logging
 import openai
@@ -51,15 +51,15 @@
         self.model = model
         self.system: Message | None = None
         self.user_prompt: List[Message] = []
         self.model_response = None
         self.usage: Usage = {"prompt_tokens": 0, "completion_tokens": 0}
         self.detailed_usage: List[DetailedUsage] = []
 
-    def _add_token_count(self,  prompt_tokens: int, completion_tokens: int, model: str) -> None:
+    def _add_token_count(self, prompt_tokens: int, completion_tokens: int, model: str) -> None:
         """Add token counts to the chain's total token count."""
         self.usage["prompt_tokens"] += prompt_tokens
         self.usage["completion_tokens"] += completion_tokens
         self.detailed_usage.append({
             "model": model,
             "usage": {"prompt_tokens": prompt_tokens, "completion_tokens": completion_tokens},
             "time": datetime.now()
@@ -89,15 +89,15 @@
             messages=messages, stream=stream, **params
         )
 
         if completion is None:
             return None
 
         if stream and isinstance(completion, Stream):
-            return CountStreamTokens(model, messages).wrap_stream_and_count(completion, self._add_token_count)
+            return wrap_stream_and_count(completion, model, self._add_token_count)
 
         elif isinstance(completion, ChatCompletion):
             message = completion.choices[0].message.content
             if message is None:
                 raise Exception("Response was empty. Please try again.")
 
             if not json_schema is None:
@@ -245,14 +245,15 @@
 
     def stream(
         self, plain_text_stream: bool = False,
         **params: Unpack[RequestParams]
     ) -> Generator[str, None, None]:
         """Returns a generator that yields responses from the LLM."""
         params['model'] = params.get('model', self.model)
+        params['stream_options'] = {'include_usage': True}
 
         if len(self.user_prompt) == 0:
             raise ValueError(
                 "User prompt is empty. Please set a user prompt before pulling."
             )
 
         return (
```

### Comparing `flowchat-1.2.3/flowchat/types.py` & `flowchat-1.2.4/flowchat/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,41 +5,68 @@
 from typing import List, NotRequired,  TypedDict, Literal, Any, Union, Dict
 from datetime import datetime
 
 
 StreamChatCompletion = Stream[ChatCompletionChunk]
 CreateResponse = None | ChatCompletion | StreamChatCompletion
 
-
 Message = TypedDict(
     'Message', {'role': str, 'content': str | List[Any]}
 )
 ResponseFormat = TypedDict(
     'ResponseFormat', {'type': Literal['text', 'json_object']})
 ImageFormat = TypedDict('ImageFormat', {
     'url': str | PILImage,
     'format_type': str,
     'detail': Literal['low', 'high']
 })
 
-# use total=False to make fields non-required
+StreamOptions = TypedDict('StreamOptions', {
+    'include_usage': bool
+})
+
+Function = TypedDict('Function', {
+    'name': str,
+    'description': NotRequired[str],
+    'parameters': NotRequired[Any],
+})
+
+Tool = TypedDict('Tool', {
+    'type': str,
+    'function': Function
+})
+
+ToolChoiceFunction = TypedDict('ToolChoiceFunction', {
+    'name': str
+})
+
+ToolChoice = TypedDict('ToolChoice', {
+    'type': str,
+    'function': ToolChoiceFunction
+})
 
 
 class RequestParams(TypedDict, total=False):
     model: NotRequired[str]
     frequency_penalty: NotRequired[Union[float, int]]
     logit_bias: NotRequired[Dict[str, Union[float, int]]]
+    logprobs: NotRequired[bool]
+    top_logprobs: NotRequired[int]
     max_tokens: NotRequired[Union[float, int]]
     n: NotRequired[Union[float, int]]
     presence_penalty: NotRequired[Union[float, int]]
     response_format: NotRequired[ResponseFormat]
     seed: NotRequired[int]
     stop: NotRequired[Union[str, List[str]]]
+    stream_options: NotRequired[StreamOptions]
     temperature: NotRequired[Union[float, int]]
     top_p: NotRequired[Union[float, int]]
+    tools: NotRequired[List[Tool]]
+    tool_choice: NotRequired[Union[str, ToolChoice]]
+    user: NotRequired[str]
 
 
 class Usage(TypedDict):
     prompt_tokens: int
     completion_tokens: int
```

### Comparing `flowchat-1.2.3/flowchat.egg-info/PKG-INFO` & `flowchat-1.2.4/flowchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.2.3
+Version: 1.2.4
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
 Requires-Dist: Pillow
-Requires-Dist: tiktoken
 Requires-Dist: requests
 
 # flowchat - clean, readable, logical code.
 
 [![PyPI version](https://img.shields.io/pypi/v/flowchat.svg)](https://pypi.org/project/flowchat/)
 [![License](https://img.shields.io/pypi/l/flowchat?logoColor=blue)](LICENSE.txt)
 ![Downloads](https://img.shields.io/pypi/dm/flowchat?logoColor=blue)
```

### Comparing `flowchat-1.2.3/setup.py` & `flowchat-1.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '1.2.3'
+VERSION = '1.2.4'
 DESCRIPTION = 'Streamlining the process of multi-prompting LLMs with chains'
 
 setup(
     name="flowchat",
     version=VERSION,
     author="Hinson Chan",
     author_email="<yhc3141@gmail.com>",
     maintainer="Hinson Chan",
     maintainer_email="<yhc3141@gmail.com>",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
-        "openai", "Pillow", "tiktoken", "requests"
+        "openai", "Pillow", "requests"
     ],
     setup_requires=['pytest-runner', 'flake8'],
     tests_require=['pytest'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

### Comparing `flowchat-1.2.3/tests/test_autodedent.py` & `flowchat-1.2.4/tests/test_autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.3/tests/test_chaining.py` & `flowchat-1.2.4/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.3/tests/test_config.py` & `flowchat-1.2.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.3/tests/test_pull.py` & `flowchat-1.2.4/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.3/tests/test_stream.py` & `flowchat-1.2.4/tests/test_stream.py`

 * *Files identical despite different names*

