# Comparing `tmp/unionllm-0.1.0.tar.gz` & `tmp/unionllm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unionllm-0.1.0.tar", last modified: Wed May  8 02:35:29 2024, max compression
+gzip compressed data, was "unionllm-0.1.1.tar", last modified: Thu May 16 03:38:25 2024, max compression
```

## Comparing `unionllm-0.1.0.tar` & `unionllm-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,59 @@
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-08 02:35:29.959463 unionllm-0.1.0/
--rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 unionllm-0.1.0/LICENSE
--rw-r--r--   0 everfly    (501) staff       (20)      446 2024-05-08 02:35:29.959277 unionllm-0.1.0/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)       81 2024-05-08 02:19:48.000000 unionllm-0.1.0/README.md
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-08 02:35:29.954445 unionllm-0.1.0/examples/
--rw-r--r--   0 everfly    (501) staff       (20)       46 2024-05-08 02:19:48.000000 unionllm-0.1.0/examples/example_usage.py
--rw-r--r--   0 everfly    (501) staff       (20)      406 2024-05-08 02:19:48.000000 unionllm-0.1.0/pyproject.toml
--rw-r--r--   0 everfly    (501) staff       (20)      140 2024-04-07 09:38:02.000000 unionllm-0.1.0/requirements.txt
--rw-r--r--   0 everfly    (501) staff       (20)       38 2024-05-08 02:35:29.959504 unionllm-0.1.0/setup.cfg
--rw-r--r--   0 everfly    (501) staff       (20)      526 2024-05-08 02:19:48.000000 unionllm-0.1.0/setup.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-08 02:35:29.955972 unionllm-0.1.0/tests/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.0/tests/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)       64 2024-05-08 02:19:48.000000 unionllm-0.1.0/tests/test_api.py
--rw-r--r--   0 everfly    (501) staff       (20)     1999 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)      979 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     1415 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)      745 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_litellm.py
--rw-r--r--   0 everfly    (501) staff       (20)     2349 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2881 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     1685 2024-05-08 02:19:48.000000 unionllm-0.1.0/tests/test_moonshot2.py
--rw-r--r--   0 everfly    (501) staff       (20)     1865 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     1946 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     1910 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     1554 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)     1404 2024-05-08 02:19:37.000000 unionllm-0.1.0/tests/test_zhipu2.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-08 02:35:29.956494 unionllm-0.1.0/unionllm/
--rw-r--r--   0 everfly    (501) staff       (20)       26 2024-05-08 02:30:49.000000 unionllm-0.1.0/unionllm/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)      306 2024-03-19 10:47:10.000000 unionllm-0.1.0/unionllm/exceptions.py
--rw-r--r--   0 everfly    (501) staff       (20)     3458 2024-05-08 02:23:33.000000 unionllm-0.1.0/unionllm/main.py
--rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 unionllm-0.1.0/unionllm/models.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-08 02:35:29.959022 unionllm-0.1.0/unionllm/providers/
--rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.0/unionllm/providers/__init__.py
--rw-r--r--   0 everfly    (501) staff       (20)     5260 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/baichuan.py
--rw-r--r--   0 everfly    (501) staff       (20)     1671 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/base_provider.py
--rw-r--r--   0 everfly    (501) staff       (20)     9733 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/coze.py
--rw-r--r--   0 everfly    (501) staff       (20)     7615 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/dify.py
--rw-r--r--   0 everfly    (501) staff       (20)     7180 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/fastgpt.py
--rw-r--r--   0 everfly    (501) staff       (20)     2409 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/litellm.py
--rw-r--r--   0 everfly    (501) staff       (20)     4904 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/minimax.py
--rw-r--r--   0 everfly    (501) staff       (20)     2641 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/moonshot.py
--rw-r--r--   0 everfly    (501) staff       (20)     6738 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/qwen.py
--rw-r--r--   0 everfly    (501) staff       (20)     5964 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/tiangong.py
--rw-r--r--   0 everfly    (501) staff       (20)     6420 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/wenxin.py
--rw-r--r--   0 everfly    (501) staff       (20)     9368 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/xunfei.py
--rw-r--r--   0 everfly    (501) staff       (20)     2366 2024-05-08 02:19:37.000000 unionllm-0.1.0/unionllm/providers/zhipu.py
--rw-r--r--   0 everfly    (501) staff       (20)    14435 2024-04-26 08:53:37.000000 unionllm-0.1.0/unionllm/utils.py
-drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-08 02:35:29.957110 unionllm-0.1.0/unionllm.egg-info/
--rw-r--r--   0 everfly    (501) staff       (20)      446 2024-05-08 02:35:29.000000 unionllm-0.1.0/unionllm.egg-info/PKG-INFO
--rw-r--r--   0 everfly    (501) staff       (20)     1053 2024-05-08 02:35:29.000000 unionllm-0.1.0/unionllm.egg-info/SOURCES.txt
--rw-r--r--   0 everfly    (501) staff       (20)        1 2024-05-08 02:35:29.000000 unionllm-0.1.0/unionllm.egg-info/dependency_links.txt
--rw-r--r--   0 everfly    (501) staff       (20)       69 2024-05-08 02:35:29.000000 unionllm-0.1.0/unionllm.egg-info/requires.txt
--rw-r--r--   0 everfly    (501) staff       (20)       15 2024-05-08 02:35:29.000000 unionllm-0.1.0/unionllm.egg-info/top_level.txt
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:38:25.385224 unionllm-0.1.1/
+-rw-r--r--   0 everfly    (501) staff       (20)       44 2024-03-19 10:47:10.000000 unionllm-0.1.1/LICENSE
+-rw-r--r--   0 everfly    (501) staff       (20)      491 2024-05-16 03:38:25.385044 unionllm-0.1.1/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)       81 2024-05-08 02:19:48.000000 unionllm-0.1.1/README.md
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:38:25.380591 unionllm-0.1.1/cookbook/
+-rw-r--r--   0 everfly    (501) staff       (20)     1752 2024-05-12 16:23:53.000000 unionllm-0.1.1/cookbook/chat_with_zhipu.ipynb
+-rw-r--r--   0 everfly    (501) staff       (20)     8970 2024-05-08 17:11:35.000000 unionllm-0.1.1/cookbook/coze_non_stream.ipynb
+-rw-r--r--   0 everfly    (501) staff       (20)    11763 2024-05-12 22:37:43.000000 unionllm-0.1.1/cookbook/coze_non_stream_func.ipynb
+-rw-r--r--   0 everfly    (501) staff       (20)    82911 2024-05-12 09:05:55.000000 unionllm-0.1.1/cookbook/test_generation_by_coze_eval_by_chatglm_faithfulness.ipynb
+-rw-r--r--   0 everfly    (501) staff       (20)    29653 2024-05-12 09:05:53.000000 unionllm-0.1.1/cookbook/test_zeval.ipynb
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:38:25.380723 unionllm-0.1.1/examples/
+-rw-r--r--   0 everfly    (501) staff       (20)       46 2024-05-08 02:19:48.000000 unionllm-0.1.1/examples/example_usage.py
+-rw-r--r--   0 everfly    (501) staff       (20)      427 2024-05-16 03:38:19.000000 unionllm-0.1.1/pyproject.toml
+-rw-r--r--   0 everfly    (501) staff       (20)      133 2024-05-12 14:58:23.000000 unionllm-0.1.1/pytest.ini
+-rw-r--r--   0 everfly    (501) staff       (20)       95 2024-05-16 03:33:55.000000 unionllm-0.1.1/requirements.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       38 2024-05-16 03:38:25.385259 unionllm-0.1.1/setup.cfg
+-rw-r--r--   0 everfly    (501) staff       (20)      563 2024-05-16 03:36:55.000000 unionllm-0.1.1/setup.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:38:25.382101 unionllm-0.1.1/tests/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.1/tests/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1409 2024-05-12 15:47:41.000000 unionllm-0.1.1/tests/test_baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1403 2024-05-13 00:05:32.000000 unionllm-0.1.1/tests/test_coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1423 2024-05-12 23:54:14.000000 unionllm-0.1.1/tests/test_dify.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1406 2024-05-12 23:47:08.000000 unionllm-0.1.1/tests/test_fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1137 2024-05-13 00:21:07.000000 unionllm-0.1.1/tests/test_litellm.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1422 2024-05-12 23:15:34.000000 unionllm-0.1.1/tests/test_minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1407 2024-05-12 15:50:43.000000 unionllm-0.1.1/tests/test_moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1377 2024-05-12 22:48:43.000000 unionllm-0.1.1/tests/test_qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1457 2024-05-12 15:56:14.000000 unionllm-0.1.1/tests/test_tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     4838 2024-05-16 03:29:43.000000 unionllm-0.1.1/tests/test_unionchat.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1444 2024-05-12 16:01:29.000000 unionllm-0.1.1/tests/test_wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1021 2024-05-12 16:19:20.000000 unionllm-0.1.1/tests/test_xunfei.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1371 2024-05-12 22:47:46.000000 unionllm-0.1.1/tests/test_zhipu.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:38:25.382608 unionllm-0.1.1/unionllm/
+-rw-r--r--   0 everfly    (501) staff       (20)       54 2024-05-09 01:57:24.000000 unionllm-0.1.1/unionllm/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)      302 2024-05-12 09:13:50.000000 unionllm-0.1.1/unionllm/exceptions.py
+-rw-r--r--   0 everfly    (501) staff       (20)     4049 2024-05-16 03:23:15.000000 unionllm-0.1.1/unionllm/main.py
+-rw-r--r--   0 everfly    (501) staff       (20)     1195 2024-03-19 10:47:10.000000 unionllm-0.1.1/unionllm/models.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:38:25.384685 unionllm-0.1.1/unionllm/providers/
+-rw-r--r--   0 everfly    (501) staff       (20)        0 2024-03-19 10:47:10.000000 unionllm-0.1.1/unionllm/providers/__init__.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5579 2024-05-12 10:20:45.000000 unionllm-0.1.1/unionllm/providers/baichuan.py
+-rw-r--r--   0 everfly    (501) staff       (20)     3484 2024-05-16 03:12:50.000000 unionllm-0.1.1/unionllm/providers/base_provider.py
+-rw-r--r--   0 everfly    (501) staff       (20)    10431 2024-05-14 02:35:52.000000 unionllm-0.1.1/unionllm/providers/coze.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7740 2024-05-12 23:53:57.000000 unionllm-0.1.1/unionllm/providers/dify.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7162 2024-05-14 02:35:50.000000 unionllm-0.1.1/unionllm/providers/fastgpt.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2119 2024-05-13 16:15:14.000000 unionllm-0.1.1/unionllm/providers/litellm.py
+-rw-r--r--   0 everfly    (501) staff       (20)     5247 2024-05-12 22:57:26.000000 unionllm-0.1.1/unionllm/providers/minimax.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2832 2024-05-13 16:15:40.000000 unionllm-0.1.1/unionllm/providers/moonshot.py
+-rw-r--r--   0 everfly    (501) staff       (20)     7055 2024-05-12 10:20:45.000000 unionllm-0.1.1/unionllm/providers/qwen.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6425 2024-05-12 16:00:03.000000 unionllm-0.1.1/unionllm/providers/tiangong.py
+-rw-r--r--   0 everfly    (501) staff       (20)     6891 2024-05-16 03:05:33.000000 unionllm-0.1.1/unionllm/providers/wenxin.py
+-rw-r--r--   0 everfly    (501) staff       (20)     9372 2024-05-12 10:04:56.000000 unionllm-0.1.1/unionllm/providers/xunfei.py
+-rw-r--r--   0 everfly    (501) staff       (20)     2533 2024-05-16 03:04:34.000000 unionllm-0.1.1/unionllm/providers/zhipu.py
+-rw-r--r--   0 everfly    (501) staff       (20)    14331 2024-05-13 16:45:47.000000 unionllm-0.1.1/unionllm/utils.py
+drwxr-xr-x   0 everfly    (501) staff       (20)        0 2024-05-16 03:38:25.384825 unionllm-0.1.1/unionllm.egg-info/
+-rw-r--r--   0 everfly    (501) staff       (20)      491 2024-05-16 03:38:25.000000 unionllm-0.1.1/unionllm.egg-info/PKG-INFO
+-rw-r--r--   0 everfly    (501) staff       (20)     1257 2024-05-16 03:38:25.000000 unionllm-0.1.1/unionllm.egg-info/SOURCES.txt
+-rw-r--r--   0 everfly    (501) staff       (20)        1 2024-05-16 03:38:25.000000 unionllm-0.1.1/unionllm.egg-info/dependency_links.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       84 2024-05-16 03:38:25.000000 unionllm-0.1.1/unionllm.egg-info/requires.txt
+-rw-r--r--   0 everfly    (501) staff       (20)       15 2024-05-16 03:38:25.000000 unionllm-0.1.1/unionllm.egg-info/top_level.txt
```

### Comparing `unionllm-0.1.0/setup.py` & `unionllm-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='unionllm',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     license='MIT',
     description='A Python library for unified access to Chinese domestic large language models.',
     author='everfly',
     author_email='tagriver@gmail.com',
     url='https://github.com/EvalsOne/UnionLLM',
     install_requires=[
         'openai',
         'pydantic',
         'zhipuai',
         'tenacity',
         'dashscope',
         'websocket_client',
-        'requests'
+        'requests',
+        'pytest',
+        'litellm'
     ],
 )
```

### Comparing `unionllm-0.1.0/tests/test_baichuan.py` & `unionllm-0.1.1/tests/test_wenxin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,39 @@
 import sys
 import os
-import unittest
+import json
+import pytest
+from dotenv import load_dotenv
+load_dotenv()
 
 # 将项目根目录添加到sys.path中
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-from unionllm.providers.baichuan import BaiChuanAIProvider, BaiChuanOpenAIError
+from unionllm.providers.wenxin import WenXinAIProvider, WenXinOpenAIError
 
-
-class TestBaiChuanProvider(unittest.TestCase):
-    def setUp(self):
-        # 请将'your_api_key'替换为您的Zhipu AI API密钥
-        self.provider = BaiChuanAIProvider(
-            api_key="sk-42c0206e207bc39c2367964e76da72ff",
-        )
-
-    def test_completion(self):
-        model = "Baichuan2-Turbo"
-        messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
+class TestWenxinAIProvider:
+    @pytest.fixture(autouse=True)
+    def setup_provider(self):
+        # 从环境变量中导入API密钥
+        self.provider = WenXinAIProvider(client_id=os.getenv("WENXIN_CLIENT_ID"), client_secret=os.getenv("WENXIN_CLIENT_SECRET"))
+
+    def test_completion_stream(self):
+        # Test non-stream completion
+        model = "ERNIE-3.5-8K"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]        
         try:
-            response = self.provider.completion(model=model, messages=messages)
-            print("response: ", response)
-            self.assertIsNotNone(response)
-        except BaiChuanOpenAIError as e:
-            raise e
-
-    # def test_completion(self):
-    #     model = "Baichuan2-Turbo"
-    #     messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
-    #     response = self.provider.completion(model=model, messages=messages, stream=True)
-    #     for chunk in response:
-    #         delta = chunk["choices"][0]["delta"]
-    #         line = {
-    #             "choices": [
-    #                 {
-    #                     "delta": {
-    #                         "role": delta["role"],
-    #                         "content": delta["content"],
-    #                     }
-    #                 }
-    #             ]
-    #         }
-    #         if "usage" in chunk:
-    #             usage_info = chunk["usage"]
-    #             line["usage"] = {
-    #                 "total_tokens": usage_info["total_tokens"],
-    #                 "prompt_tokens": usage_info["prompt_tokens"],
-    #                 "completion_tokens": usage_info["completion_tokens"],
-    #             }
-    #         print("line: ", line)
-    #     self.assertIsNotNone(response)
-
-
-if __name__ == "__main__":
-    unittest.main()
+            response = self.provider.completion(model=model, messages=messages, stream=True)
+            for chunk in response:
+                print(chunk["choices"][0]["delta"]["content"])
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
+        
+
+    def test_completion_non_stream(self):
+        # 定义模型和消息
+        model = "ERNIE-3.5-8K"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=False)
+            print(response)
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
```

### Comparing `unionllm-0.1.0/tests/test_fastgpt.py` & `unionllm-0.1.1/tests/test_moonshot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 import sys
 import os
-import unittest
 import json
+import pytest
+from dotenv import load_dotenv
+load_dotenv()
 
 # 将项目根目录添加到sys.path中
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-from unionllm.providers.fastgpt import FastGPTProvider
+from unionllm.providers.moonshot import MoonshotAIProvider, MoonshotOpenAIError
 
+class TestMoonshotAIProvider:
+    @pytest.fixture(autouse=True)
+    def setup_provider(self):
+        # 从环境变量中导入API密钥
+        self.provider = MoonshotAIProvider(api_key=os.getenv("MOONSHOT_API_KEY"))
+
+    def test_completion_stream(self):
+        # Test non-stream completion
+        model = "moonshot-v1-8k"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]        
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=True)
+            for chunk in response:
+                print(chunk["choices"][0]["delta"]["content"])
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
+        
 
-class TestFastGPTProvider(unittest.TestCase):
-    def setUp(self):
-        # 请将'your_api_key'替换为您的Zhipu AI API密钥
-        self.provider = FastGPTProvider(
-            api_key="fastgpt-iiCmNijSSN6Mvkr3LOv1tICdlVeVVhUlgSP7QUaiZMgXeXBhM4SzJPvyx4vVT"
-        )
-
-    # def test_completion_non_stream_success(self):
-    #     # Test non-stream completion
-    #     model = "fastgpt"
-    #     messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
-    #     response = self.provider.completion(model=model, messages=messages, stream=True, details=True)
-
-    #     print("stream response: ", response)
-
-    #     # 检查捕获的异常是否符合预期
-    #     self.assertIsNotNone(response)
-
-    def test_completion_non_stream_failure(self):
-
+    def test_completion_non_stream(self):
         # 定义模型和消息
-        model = "fastgpt"
-        messages = [{"content": "财商测试", "role": "user"}]
-
-        response = self.provider.completion(model=model, messages=messages, stream=False, details=True)
-
-        print("response: ", response)
-
-        # 检查捕获的异常是否符合预期
-        self.assertIsNotNone(response)
-
-if __name__ == "__main__":
-    unittest.main()
+        model = "moonshot-v1-8k"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=False)
+            print(response)
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
```

### Comparing `unionllm-0.1.0/tests/test_qwen.py` & `unionllm-0.1.1/tests/test_coze.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,40 @@
 import sys
 import os
-import unittest
 import json
-import dashscope
+import pytest
+from dotenv import load_dotenv
+load_dotenv()
 
 # 将项目根目录添加到sys.path中
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-from unionllm.providers.qwen import QwenAIProvider
+from unionllm.providers.coze import CozeAIProvider, CozeAIError
 
-
-class TestQwenAIProvider(unittest.TestCase):
-    def setUp(self):
-        self.provider = QwenAIProvider(api_key="sk-45ad8752a48d47ffaf86f5b000eff589")
-
-    def test_completion(self):
-        model = "qwen-turbo"
-        messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
-        response = self.provider.completion(model=model, messages=messages)
-        print("response: ", response)
-        self.assertIsNotNone(response)
-
-    # def test_completion(self):
-    #     model = "qwen-turbo"
-    #     messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
-    #     response = self.provider.completion(model=model, messages=messages, stream=True)
-    #     for chunk in response:
-    #         new_chunk = json.loads(chunk)
-    #         delta = new_chunk["choices"][0]["delta"]
-    #         line = {
-    #             "choices": [
-    #                 {
-    #                     "delta": {
-    #                         "role": delta["role"],
-    #                         "content": delta["content"],
-    #                     }
-    #                 }
-    #             ]
-    #         }
-    #         if "usage" in new_chunk:
-    #             usage_info = new_chunk["usage"]
-    #             line["usage"] = {
-    #                 "prompt_tokens": usage_info["prompt_tokens"],
-    #                 "completion_tokens": usage_info["completion_tokens"],
-    #                 "total_tokens": usage_info["total_tokens"],
-    #             }
-    #         print("line:", line)
-    #     self.assertIsNotNone(response)
-
-
-if __name__ == "__main__":
-    unittest.main()
+class TestCozeAIProvider:
+    @pytest.fixture(autouse=True)
+    def setup_provider(self):
+        # 从环境变量中导入API密钥
+        self.provider = CozeAIProvider(api_key=os.getenv("COZE_API_KEY"), bot_id=os.getenv("COZE_BOT_ID"))
+
+    def test_completion_stream(self):
+        # Test non-stream completion
+        model = "coze"
+        messages = [{"content": "瑞文智商测试", "role": "user"}]        
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=True)
+            for chunk in response:
+                if chunk.choices:
+                    print(chunk.choices[0].delta.content)
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
+        
+
+    def test_completion_non_stream(self):
+        # 定义模型和消息
+        model = "coze"
+        messages = [{"content": "瑞文智商测试", "role": "user"}]
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=False)
+            print(response)
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
```

### Comparing `unionllm-0.1.0/tests/test_wenxin.py` & `unionllm-0.1.1/tests/test_tiangong.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,39 @@
-import json
 import sys
 import os
-import unittest
+import json
+import pytest
+from dotenv import load_dotenv
+load_dotenv()
 
 # 将项目根目录添加到sys.path中
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-from unionllm.providers.wenxin import WenXinAIProvider
-
-
-class TestWenXinProvider(unittest.TestCase):
-    def setUp(self):
-        # 请将'your_api_key'替换为您的Zhipu AI API密钥
-        self.provider = WenXinAIProvider(
-            api_key="AvA4gBP5LZqKEruKGYzfYzU9",
-            secret_key="8Mg2XN3zPmskxzeYY3i7P7u24poGIHmO",
-        )
-
-    def test_completion(self):
-        model = "completions_pro"
-        messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
-        response = self.provider.completion(model=model, messages=messages)
-        print("response: ", response)
-        self.assertIsNotNone(response)
-
-    # def test_completion(self):
-    #     model = "completions_pro"
-    #     messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
-    #     response = self.provider.completion(model=model, messages=messages, stream=True)
-    #     for chunk in response:
-    #         delta = chunk["choices"][0]["delta"]
-    #         line = {
-    #             "choices": [
-    #                 {
-    #                     "delta": {
-    #                         "role": delta["role"],
-    #                         "content": delta["content"],
-    #                     }
-    #                 }
-    #             ]
-    #         }
-    #         if "usage" in chunk:
-    #             line["usage"] = {
-    #                 "prompt_tokens": chunk["usage"]["prompt_tokens"],
-    #                 "completion_tokens": chunk["usage"]["completion_tokens"],
-    #                 "total_tokens": chunk["usage"]["total_tokens"],
-    #             }
-    #         print("line: ", line)
-    #     self.assertIsNotNone(response)
-
+from unionllm.providers.tiangong import TianGongAIProvider, TianGongAIProvider
 
-if __name__ == "__main__":
-    unittest.main()
+class TestTianGongAIProvider:
+    @pytest.fixture(autouse=True)
+    def setup_provider(self):
+        # 从环境变量中导入API密钥
+        self.provider = TianGongAIProvider(api_key=os.getenv("TIANGONG_API_KEY"), api_secret=os.getenv("TIANGONG_API_SECRET"))
+
+    def test_completion_stream(self):
+        # Test non-stream completion
+        model = "SkyChat-MegaVerse"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]        
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=True)
+            for chunk in response:
+                print(chunk["choices"][0]["delta"]["content"])
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
+        
+
+    def test_completion_non_stream(self):
+        # 定义模型和消息
+        model = "SkyChat-MegaVerse"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=False)
+            print(response)
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
```

### Comparing `unionllm-0.1.0/tests/test_zhipu.py` & `unionllm-0.1.1/unionllm/models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,28 @@
-import sys
-import os
-import unittest
-import json
+from typing import List, Optional
 
-# 将项目根目录添加到sys.path中
-sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
-
-from unionllm.providers.zhipu import ZhipuAIProvider
-
-
-class TestZhipuAIProvider(unittest.TestCase):
-    def setUp(self):
-        # 请将'your_api_key'替换为您的Zhipu AI API密钥
-        self.provider = ZhipuAIProvider(
-            api_key="38dc046c622b6ec1b9bfa0413e6ca2ee.2Yn3uFr8j74pMOvK"
-        )
-
-    def test_completion(self):
-        model = "GLM-4"
-        messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
-        response = self.provider.completion(model=model, messages=messages)
-        for chunk in response:
-            print("chunk: ", chunk)
-            delta = chunk.choices[0].delta
-            line = {
-                "choices": [
-                    {
-                        "delta": {
-                            "role": delta.role,
-                            "content": delta.content,
-                        }
-                    }
-                ]
-            }
-            if chunk.usage is not None:
-                line["usage"] = {
-                    "prompt_tokens": chunk.usage.prompt_tokens,
-                    "completion_tokens": chunk.usage.completion_tokens,
-                    "total_tokens": chunk.usage.total_tokens,
-                }
-            print("line内容2: ", line)
-        print("response: ", response)
-        self.assertIsNotNone(response)
-
-if __name__ == "__main__":
-    unittest.main()
+class ResponseModel:
+    def __init__(self, prompt_tokens: List[str], completion_tokens: List[str], total_tokens: int, total_attempts: int, raw_response: Optional[dict] = None, usage: Optional[dict] = None):
+        self.prompt_tokens = prompt_tokens
+        self.completion_tokens = completion_tokens
+        self.total_tokens = total_tokens
+        self.total_attempts = total_attempts
+        self.raw_response = raw_response
+        self.usage = usage
+
+    def to_dict(self) -> dict:
+        return {
+            "prompt_tokens": self.prompt_tokens,
+            "completion_tokens": self.completion_tokens,
+            "total_tokens": self.total_tokens,
+            "total_attempts": self.total_attempts,
+            "raw_response": self.raw_response,
+            "usage": self.usage
+        }
+
+    def get_completions(self) -> list[str]:
+        completions = []
+        if self.raw_response and "choices" in self.raw_response:
+            for choice in self.raw_response["choices"]:
+                if "message" in choice and "content" in choice["message"]:
+                    completions.append(choice["message"]["content"])
+        return completions
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `unionllm-0.1.0/tests/test_zhipu2.py` & `unionllm-0.1.1/tests/test_baichuan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 import sys
 import os
-import unittest
 import json
-from unittest.mock import patch, MagicMock
+import pytest
+from dotenv import load_dotenv
+load_dotenv()
 
 # 将项目根目录添加到sys.path中
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 
-from unionllm.providers.zhipu import ZhipuAIProvider, ZhiPuOpenAIError
+from unionllm.providers.baichuan import BaiChuanAIProvider, BaiChuanOpenAIError
 
-class TestZhipuAIProvider(unittest.TestCase):
-    def setUp(self):
-        # 请将'your_api_key'替换为您的Zhipu AI API密钥
-        self.provider = ZhipuAIProvider(api_key="38dc046c622b6ec1b9bfa0413e6ca2ee.2Yn3uFr8j74pMOvK")
+class TestBaichuanAIProvider:
+    @pytest.fixture(autouse=True)
+    def setup_provider(self):
+        # 从环境变量中导入API密钥
+        self.provider = BaiChuanAIProvider(api_key=os.getenv("BAICHUAN_API_KEY"))
 
-    def test_completion_non_stream_success(self):
+    def test_completion_stream(self):
         # Test non-stream completion
-        model = "GLM-4"
-        messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
-        response = self.provider.completion(model=model, messages=messages, stream=True)
-
-        print("stream response: ", response)
-
-        # 检查捕获的异常是否符合预期
-        self.assertIsNotNone(response)
-
-    def test_completion_non_stream_failure(self):
+        model = "Baichuan2-Turbo"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]        
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=True)
+            for chunk in response:
+                print(chunk["choices"][0]["delta"]["content"])
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
+        
 
+    def test_completion_non_stream(self):
         # 定义模型和消息
-        model = "GLM-4"
-        messages = [{"content": "你好，今天天气怎么样？", "role": "user"}]
-
-        response = self.provider.completion(model=model, messages=messages, stream=False)
-
-        print("response: ", response)
-
-        # 检查捕获的异常是否符合预期
-        self.assertIsNotNone(response)
-
-if __name__ == "__main__":
-    unittest.main()
+        model = "Baichuan2-Turbo"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=False)
+            print(response)
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
```

### Comparing `unionllm-0.1.0/unionllm/main.py` & `unionllm-0.1.1/unionllm/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Any, List
-from .providers import base_provider
 from .providers import zhipu, moonshot, minimax, qwen, tiangong, baichuan, wenxin, xunfei, dify, fastgpt, coze, litellm
 from .exceptions import ProviderError
+from litellm import completion as litellm_completion
 
 logger = logging.getLogger(__name__)
 
 class UnionLLM:
     def __init__(self, provider: str, **kwargs):
         self.provider = provider.lower()
         self.litellm_call_type = None
@@ -28,40 +28,50 @@
             self.provider_instance = xunfei.XunfeiAIProvider(**kwargs)
         elif self.provider == "dify":
             self.provider_instance = dify.DifyAIProvider(**kwargs)
         elif self.provider == "fastgpt":
             self.provider_instance = fastgpt.FastGPTProvider(**kwargs)
         elif self.provider == "coze":
             self.provider_instance = coze.CozeAIProvider(**kwargs)
-        else:
+        elif self.provider:
             if_litellm_support, support_type = self.check_litellm_providers(provider=self.provider)
             if if_litellm_support:
                 self.provider_instance = litellm.LiteLLMProvider(**kwargs)
                 if support_type == 1:
                     self.litellm_call_type = 1
                 elif support_type == 2:
                     self.litellm_call_type = 2
             else:
                 raise ProviderError(f"Provider '{self.provider}' is not supported.")
+        else:
+            self.provider_instance = litellm.LiteLLMProvider(**kwargs)
 
     def completion(self, model: str, messages: List[str], **kwargs) -> Any:
         if not self.provider_instance:
             raise ProviderError(f"Provider '{self.provider}' is not initialized.")
         
         if self.litellm_call_type:
             if self.litellm_call_type == 1:
-                # 判断model是否以self.provider开头，如果不是则加上
-                if not model.startswith(self.provider):
+                # Jugde whether the model starts with self.provider, if not, add it
+                if not model.startswith(self.provider+"/"):
                     model = f"{self.provider}/{model}"
                 return self.provider_instance.completion(model, messages, **kwargs)
             elif self.litellm_call_type == 2:
                 return self.provider_instance.completion(model, messages, **kwargs)
         else:
             return self.provider_instance.completion(model, messages, **kwargs)
         
     def check_litellm_providers(self, provider: str) -> bool:
+        # Judge whether the provider is supported by LiteLLM, and if provider name should be added to the model name
         if provider in ['azure', 'sagemaker', 'bedrock', 'vertex_ai', 'palm', 'gemini', 'mistral', 'cloudflare', 'huggingface', 'replicate', 'together_ai', 'openrouter', 'baseten', 'nlp_cloud', 'petals', 'ollama', 'perplexity', 'groq', 'anyscale', 'watsonx', 'voyage', 'xinference']:
+            # provider name should be added to the model name
             return True, 1
         elif provider in ['openai', 'claude', 'cohere', 'ai21', 'luminous']:
+            # provider name should not be added to the model name
             return True, 2
         else:
-            return False, 0
+            return False, 0
+        
+# This is the new function to simplify calling
+def unionchat(model: str, messages: List[dict], **kwargs) -> Any:
+    client = UnionLLM(**kwargs)
+    return client.completion(model=model, messages=messages, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `unionllm-0.1.0/unionllm/providers/baichuan.py` & `unionllm-0.1.1/unionllm/providers/baichuan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import json
 from .base_provider import BaseProvider
 from unionllm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
 import requests
-import logging
+import logging, os
 
 class BaiChuanOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
 class BaiChuanAIProvider(BaseProvider):
-    def __init__(self, **model_kwargs):
-        self.api_key = model_kwargs.get("api_key")
+    def __init__(self, **model_kwargs):        
+        # Get BAICHUAN_API_KEY from environment variables
+        _env_api_key = os.environ.get("BAICHUAN_API_KEY")
+        self.api_key = model_kwargs.get("api_key") if model_kwargs.get("api_key") else _env_api_key
+        if not self.api_key:
+            raise BaiChuanOpenAIError(
+                status_code=422, message=f"Missing API key"
+            )
         self.endpoint_url = "https://api.baichuan-ai.com/v1/chat/completions"
 
     def pre_processing(self, **kwargs):
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
```

### Comparing `unionllm-0.1.0/unionllm/providers/base_provider.py` & `unionllm-0.1.1/tests/test_fastgpt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,40 @@
-from abc import ABC, abstractmethod
-from ..models import ResponseModel
-from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, List
-from unionllm.utils import Message, Choices, Usage, ModelResponse
-
-if TYPE_CHECKING:
-    from dataclasses import dataclass
-else:
-    from pydantic.dataclasses import dataclass
-
-@dataclass
-class BaseProvider(ABC):
-    args: Optional[Dict[str, Any]] = None
-    key: Optional[str] = None
-    group: Optional[str] = None
-
-    def __init__(
-        self,
-        status_code,
-        message,
-    ):
-        self.status_code = status_code
-        self.message = message
-
-    @abstractmethod
-    def completion(self, model: str, messages: list) -> ResponseModel:
-        pass
-
-    def create_model_response(self, openai_response: Any, model: str) -> ResponseModel:
-        print("openai_response: ", openai_response)
-        choices = []
-
-        for choice in openai_response.choices:
-            print("choice.message.content: ", choice.message.content)
-            message = Message(content=choice.message.content, role=choice.message.role)
-            print("message: ", message)
-            choices.append(Choices(message=message, index=choice.index, finish_reason=choice.finish_reason))
-
-        usage = Usage(
-            prompt_tokens=openai_response.usage.prompt_tokens,
-            completion_tokens=openai_response.usage.completion_tokens,
-            total_tokens=openai_response.usage.total_tokens
-        )
-        response =  ModelResponse(
-            id=openai_response.id,
-            choices=choices,
-            created=openai_response.created,
-            model=model,
-            usage=usage
-        )
-        pass
+import sys
+import os
+import json
+import pytest
+from dotenv import load_dotenv
+load_dotenv()
+
+# 将项目根目录添加到sys.path中
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
+
+from unionllm.providers.fastgpt import FastGPTProvider, FastGPTError
+
+class TestFastGPTAIProvider:
+    @pytest.fixture(autouse=True)
+    def setup_provider(self):
+        # 从环境变量中导入API密钥
+        self.provider = FastGPTProvider(api_key=os.getenv("FASTGPT_API_KEY"))
+
+    def test_completion_stream(self):
+        # Test non-stream completion
+        model = "fastgpt"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]        
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=True)
+            for chunk in response:
+                if chunk.choices:
+                    print(chunk.choices[0].delta.content)
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
+        
+
+    def test_completion_non_stream(self):
+        # 定义模型和消息
+        model = "fastgpt"
+        messages = [{"content": "introduce yourself briefly.", "role": "user"}]
+        try:
+            response = self.provider.completion(model=model, messages=messages, stream=False)
+            print(response)
+        except Exception as e:
+            pytest.fail(f"Error occurred: {e}")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `unionllm-0.1.0/unionllm/providers/coze.py` & `unionllm-0.1.1/unionllm/providers/coze.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from .base_provider import BaseProvider
-from unionllm.utils import ResponseModelInterface
 from unionllm.utils import ModelResponse, Message, Choices, Usage, Context, generate_unique_uid, Delta, StreamingChoices
 from openai import OpenAI
-import logging, json, time, requests
+import logging, json, time, requests, os
 
 
 class CozeAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
@@ -14,15 +13,28 @@
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
 
 class CozeAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.api_key = model_kwargs.get("api_key")
+        # Get COZE_API_KEY from environment variables
+        _env_api_key = os.environ.get("COZE_API_KEY")
+        _env_bot_id = os.environ.get("COZE_BOT_ID")
+        self.api_key = model_kwargs.get("api_key") if model_kwargs.get("api_key") else _env_api_key
+        self.bot_id = model_kwargs.get("bot_id") if model_kwargs.get("bot_id") else _env_bot_id
+        if not self.api_key:
+            raise CozeAIError(
+                status_code=422, message=f"Missing API key"
+            )
+        if not self.bot_id:
+            raise CozeAIError(
+                status_code=422, message=f"Missing Bot ID"
+            )
+        
         self.base_url = "https://api.coze.com/open_api/v2"
         self.endpoint_url = self.base_url + "/chat"
 
     def pre_processing(self, **kwargs):
         # 处理参数兼容性问题，不支持的参数全部舍弃
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
@@ -31,91 +43,102 @@
         ]
         for key in list(kwargs.keys()):
             if key not in supported_params:
                 kwargs.pop(key)
         return kwargs
 
     def to_formatted_prompt(self, messages):
-        message = messages[-1]
+        last_message = messages[-1]
         # if last message role is not user, return error
-        if message["role"] != "user":
+        if last_message["role"] != "user":
             raise CozeAIError(
                 status_code=422, message=f"Last message role should be user"
             )
-        query = message["content"]
-        return messages, query
+        query = last_message["content"]
+        # 从messages去掉最后一条消息
+        history = messages[:-1]
+        history_messages = []
+        for message in history:
+            if message["role"] == "assistant":
+                # 在message中追加content_type字段和content字段
+                message["type"] = "answer"
+                message["content_type"] = "text"
+                history_messages.append(message)
+            elif message["role"] == "user":
+                message["content_type"] = "text"
+                history_messages.append(message)
+        return history_messages, query
 
     def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
         # 预处理消息内容并提取用户问题
-        messages, query = self.to_formatted_prompt(messages)
+        history, query = self.to_formatted_prompt(messages)
 
         # 接收user_id作为用户唯一标识传入参数
         if 'user_id' not in new_kwargs:
             user_id = generate_unique_uid()
         else:
             user_id = new_kwargs['user_id']
-        payload = json.dumps({"query": query,"user": user_id,"bot_id": model,"chat_history":[], "stream": True})
+        payload = json.dumps({"query": query,"user": user_id,"bot_id": self.bot_id,"chat_history":history, "stream": True})
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
         response = requests.post(self.endpoint_url, headers=headers, data=payload)
 
         for line in response.iter_lines():
             if line:
                 if line.startswith(b"data:"):
                     new_line = line.decode("utf-8").replace("data:", "")
                     if new_line == "[DONE]":
                         continue
 
                     data = json.loads(new_line)
-                    print("data is:",data)
-                    chunk_line = {}
                     chunk_context = []
                     chunk_choices = []
                     index = 0
                     if "message" in data:
                         message = data["message"]
-                        if message['role'] == 'assistant' and message['type'] == 'knowledge':
-                            # 解析知识型内容
-                            content = message['content']
+                        if message['role'] == 'assistant':
                             conversation_id = data.get('conversation_id', 0)
-                            # 假设knowledge类型内容是由"---\nrecall slice X:\n"分隔的
-                            slices = content.split('---\n')
-                            index = 0
-                            for slice in slices:
-                                if slice.strip().startswith('recall slice'):
-                                    # 去掉前缀找到JSON部分
-                                    json_part = slice.strip().split('\n', 1)[-1].strip()
-                                    # 如果不是以\"}结尾，则强制添加
-                                    if not json_part.endswith('\"}'):
-                                        json_part += '\"}'
-                                    try:
-                                        # 尝试解析JSON数据
-                                        recall_data = json.loads(json_part)
-                                        chunk_context.append({
-                                            "id": index,
-                                            "content": str(recall_data)    
-                                        })
-                                        index += 1
-                                    except json.JSONDecodeError:
-                                        raise CozeAIError(status_code=500, message=f"Error decoding JSON from slice: {json_part}")
-
-                        elif message['role'] == 'assistant' and message['type'] == 'answer':
-                            chunk_choices = []
-                            chunk_delta = Delta()
-                            if "role" in message:
-                                chunk_delta.role = message["role"]
-                            if "content" in message:
-                                chunk_delta.content = message["content"]
-                            chunk_choices.append(StreamingChoices(index=str(index), delta=chunk_delta))
+                            if message['type'] == 'knowledge':
+                                # 解析知识型内容
+                                content = message['content']
+                                # 假设knowledge类型内容是由"---\nrecall slice X:\n"分隔的
+                                slices = content.split('---\n')
+                                index = 0
+                                for slice in slices:
+                                    if slice.strip().startswith('recall slice'):
+                                        # 去掉前缀找到JSON部分
+                                        json_part = slice.strip().split('\n', 1)[-1].strip()
+                                        # 如果不是以\"}结尾，则强制添加
+                                        if not json_part.endswith('\"}'):
+                                            json_part += '\"}'
+                                        try:
+                                            # 尝试解析JSON数据
+                                            recall_data = json.loads(json_part)
+                                            chunk_context.append({
+                                                "id": index,
+                                                "content": str(recall_data)    
+                                            })
+                                            index += 1
+                                        except json.JSONDecodeError:
+                                            raise CozeAIError(status_code=500, message=f"Error decoding JSON from slice: {json_part}")
+
+                            elif message['type'] == 'answer':
+                                chunk_choices = []
+                                chunk_delta = Delta()
+                                if "role" in message:
+                                    chunk_delta.role = message["role"]
+                                if "content" in message:
+                                    chunk_delta.content = message["content"]
+                                chunk_choices.append(StreamingChoices(index=str(index), delta=chunk_delta))
                         
                         chunk_usage = Usage()
                         chunk_response = ModelResponse(
-                            id=conversation_id,
+                            id=conversation_id if conversation_id else "",
                             choices=chunk_choices,
                             context=chunk_context,
                             created=int(time.time()),
                             model=model,
                             usage=chunk_usage if chunk_usage else None,
                             stream=True
                         )
@@ -124,42 +147,30 @@
 
     def create_model_response_wrapper(self, result, model):
         choices = []
         context = []
 
         result_dict = result.json()
         messages = result_dict.get('messages', [])
+        if not messages:
+            code = result_dict.get('code', 500)
+            message = result_dict.get('msg', 'Internal Server Error')
+            raise CozeAIError(status_code=code, message=message)
         results = []
         cotext_pre = []
 
-        print("messages is:",messages)
-
         for message in messages:
             # 根据消息类型处理数据
-            if message['role'] == 'assistant' and message['type'] == 'knowledge':
+            if message['role'] == 'assistant' and message['type'] == 'verbose':
                 # 解析知识型内容
-                content = message['content']
-                print("content is:",content)
-
-                # 假设knowledge类型内容是由"---\nrecall slice X:\n"分隔的
-                slices = content.split('---\n')
-                for slice in slices:
-                    if slice.strip().startswith('recall slice'):
-                        # 去掉前缀找到JSON部分
-                        json_part = slice.strip().split('\n', 1)[-1].strip()
-                        # 如果不是以\"}结尾，则强制添加
-                        if not json_part.endswith('\"}'):
-                            json_part += '\"}'
-
-                        try:
-                            # 尝试解析JSON数据
-                            recall_data = json.loads(json_part)
-                            cotext_pre.append(str(recall_data))
-                        except json.JSONDecodeError:
-                            raise CozeAIError(status_code=500, message=f"Error decoding JSON from slice: {json_part}")
+                content = json.loads(message['content'])
+                if "verbose_type" in content and content["verbose_type"] == "knowledge":
+                    chunks = content["chunks"]
+                    for chunk in chunks:
+                        cotext_pre.append({"content":chunk["slice"],"score":chunk["score"]})
 
             elif message['role'] == 'assistant' and message['type'] == 'answer':
                 # 直接添加回复内容
                 results.append(message['content'])
 
         message = Message(
             content=results[0],
@@ -180,15 +191,15 @@
         )
 
         # Assume response_dict contains a field 'responseData' with quoteList to extract context
         if cotext_pre:
             i = 0
             for context_item in cotext_pre:
                 i += 1
-                context.append(Context(id=i, content=context_item))
+                context.append(Context(id=i, content=context_item['content'], score=context_item['score']))
 
         response = ModelResponse(
             id=result_dict.get('conversation_id'),
             choices=choices,
             context=context,
             created=int(time.time()),
             model='',
@@ -204,22 +215,22 @@
                 )
             new_kwargs = self.pre_processing(**kwargs)
             stream = kwargs.get("stream", False)
 
             if stream:
                 return self.post_stream_processing_wrapper(model, messages, **new_kwargs)
             else:
-                messages, query = self.to_formatted_prompt(messages)
+                history, query = self.to_formatted_prompt(messages)
 
                 # 接受user_id作为用户唯一身份标识传入参数
                 if 'user_id' not in kwargs:
                     user_id = generate_unique_uid()
                 else:
                     user_id = kwargs['user_id']
-                payload = json.dumps({"query": query,"user": user_id,"bot_id": model,"chat_history":[],"steam":False})
+                payload = json.dumps({"query": query,"user": user_id,"bot_id": self.bot_id,"chat_history":history,"steam":False})
 
                 headers = {
                     "Authorization": f"Bearer {self.api_key}",
                     "Content-Type": "application/json",
                 }
                 result = requests.post(self.endpoint_url, headers=headers, data=payload)
                 return self.create_model_response_wrapper(result, model=model)
```

### Comparing `unionllm-0.1.0/unionllm/providers/dify.py` & `unionllm-0.1.1/unionllm/providers/dify.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import json
 from .base_provider import BaseProvider
 from unionllm.utils import ModelResponse, Message, Choices, Usage, Context, Delta, StreamingChoices
 import requests
-import logging, json, time
+import logging, json, time, os
 
 class DifyOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
 class DifyAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.api_key = model_kwargs.get("api_key")
+        # Get DIFY_API_KEY from environment variables
+        _env_api_key = os.environ.get("DIFY_API_KEY")
+        self.api_key = model_kwargs.get("api_key") if model_kwargs.get("api_key") else _env_api_key
+        if not self.api_key:
+            raise DifyOpenAIError(
+                status_code=422, message=f"Missing API key"
+            )
         self.endpoint_url = "https://api.dify.ai/v1/chat-messages"
 
     def pre_processing(self, **kwargs):
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
@@ -64,15 +70,14 @@
                 if line.startswith(b"data:"):
                     new_line = line.decode("utf-8").replace("data: ", "")
                     if new_line == "[DONE]":
                         continue
                     
                     
                     data = json.loads(new_line)
-                    print("data is:",data)
                     event = data.get("event")
                     msg_id = data.get("message_id")
                     if event == "message":
                         if 'answer' in data:
                             chunk_message = data["answer"]
                             if chunk_message:
                                 chunk_delta.role = "assistant"
@@ -107,16 +112,14 @@
                         stream=True
                     )
                     index += 1
                     yield chunk_response
 
     def create_model_response_wrapper(self, result, model):
 
-        print("result of dify:", result.json())
-
         response_dict = result.json()
         choices = []
         context = []
 
         message = Message(
             content=response_dict['answer'], role="assistant"
         )
@@ -164,24 +167,20 @@
             if model is None or messages is None:
                 raise DifyOpenAIError(
                     status_code=422, message=f"Missing model or messages"
                 )
             new_kwargs = self.pre_processing(**kwargs)
             stream = kwargs.get("stream", False)
 
-            print("stream is:", stream)
-
             if stream:
                 return self.post_stream_processing_wrapper(model, messages, **new_kwargs)
             else:
                 messages, query = self.to_formatted_prompt(messages)
                 mode = "blocking"
 
-                print("mode is:", mode)
-
                 payload = json.dumps({"query": query, "response_mode": mode, "user": "abc-123","conversation_id": "","inputs":{}})
                 headers = {
                     "Authorization": f"Bearer {self.api_key}",
                     "Content-Type": "application/json",
                 }
                 result = requests.post(self.endpoint_url, headers=headers, data=payload)
                 return self.create_model_response_wrapper(result, model=model)
```

### Comparing `unionllm-0.1.0/unionllm/providers/fastgpt.py` & `unionllm-0.1.1/unionllm/providers/fastgpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from .base_provider import BaseProvider
-from unionllm.utils import ResponseModelInterface
 from unionllm.utils import ModelResponse, Message, Choices, Usage, Context, Delta, StreamingChoices
 from openai import OpenAI
-import logging, json, time, requests
+import logging, json, time, requests, os
 
 
 class FastGPTError(Exception):
     def __init__(
         self,
         status_code,
         message,
@@ -14,21 +13,26 @@
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
 
 class FastGPTProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.api_key = model_kwargs.get("api_key")
+        # Get FASTGPT_API_KEY from environment variables
+        _env_api_key = os.environ.get("FASTGPT_API_KEY")
+        self.api_key = model_kwargs.get("api_key") if model_kwargs.get("api_key") else _env_api_key
+        if not self.api_key:
+            raise FastGPTError(
+                status_code=422, message=f"Missing API key"
+            )
         self.base_url = "https://api.fastgpt.in/api/v1"
-        self.response_model = ResponseModelInterface()
         self.endpoint_url = self.base_url + "/chat/completions"
 
     def pre_processing(self, **kwargs):
-        # 处理参数兼容性问题，不支持的参数全部舍弃
+        # process the compatibility issue of parameters, all unsupported parameters are discarded
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
         ]
         for key in list(kwargs.keys()):
             if key not in supported_params:
@@ -50,36 +54,36 @@
             if line:
                 chunk_choices = []
                 chunk_context = []
                 if line.startswith(b"data:"):
                     new_line = line.decode("utf-8").replace("data: ", "")
                     if new_line == "[DONE]":
                         continue
-                    data = json.loads(new_line)
-                    print("data is:",data)
+                    try:
+                        data = json.loads(new_line)
+                    except Exception as e:
+                        continue
 
                     if "choices" in data:
                         chunk_message = data["choices"][0]["delta"]
                         chunk_delta = Delta()
                         if chunk_message:
                             if "role" in chunk_message:
                                 chunk_delta.role = chunk_message['role']
                             if "content" in chunk_message:
                                 chunk_delta.content = chunk_message['content']
                             chunk_choices.append(StreamingChoices(index=str(index), delta=chunk_delta))
 
-                    if "usage" in data:
-                        usage_info = data["usage"]
-                        chunk_usage = Usage()
-                        if "prompt_tokens" in usage_info:
-                            chunk_usage.prompt_tokens = usage_info["prompt_tokens"]
-                        if "completion_tokens" in usage_info:
-                            chunk_usage.completion_tokens = usage_info["completion_tokens"]
-                        if "total_tokens" in usage_info:
-                            chunk_usage.total_tokens = usage_info["total_tokens"]
+                    if isinstance(data, list):
+                        summary = data[0]
+                        if "tokens" in summary:
+                            chunk_usage = Usage()
+                            chunk_usage.total_tokens = summary['tokens']
+                        else:
+                            chunk_usage = None
                     else:
                         chunk_usage = None
 
                     if isinstance(data, list):
                         for module in data:
                             if "quoteList" in module:
                                 for quote in module["quoteList"]:
@@ -87,30 +91,28 @@
                                     chunk_context.append(
                                         {
                                             "id": quote["id"],
                                             "content": content,
                                         }    
                                     )
                 
-                    print("data", line)
                     chunk_response = ModelResponse(
                         id=data['id'] if 'id' in data else None,
                         choices=chunk_choices,
                         context=chunk_context,
                         created=int(time.time()),
                         model=model,
                         usage=chunk_usage if chunk_usage else None,
                         stream=True
                     )
                     index += 1
                     yield chunk_response
 
     def create_model_response_wrapper(self, result):
         response_dict = result.json()
-        print(response_dict)
         choices = []
         context = []
         message = Message(
             content=response_dict['choices'][0]['message']['content'],
             role="assistant"
         )
         choices.append(
```

### Comparing `unionllm-0.1.0/unionllm/providers/litellm.py` & `unionllm-0.1.1/unionllm/providers/zhipu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,67 @@
-import json, time
-import dashscope
+import json
 from .base_provider import BaseProvider
-from unionllm.utils import ResponseModelInterface
-from litellm import completion
+from zhipuai import ZhipuAI
+import logging, os
 
-class LiteLLMOpenAIError(Exception):
+class ZhiPuOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
-class LiteLLMProvider(BaseProvider):
+class ZhipuAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.api_key = model_kwargs.get("api_key")
-        self.response_model = ResponseModelInterface()
+        # Get ZHIPU_API_KEY from environment variables
+        _env_api_key = os.environ.get("ZHIPU_API_KEY")
+        self.api_key = model_kwargs.get("api_key") if model_kwargs.get("api_key") else _env_api_key
+        if not self.api_key:
+            raise ZhiPuOpenAIError(
+                status_code=422, message=f"Missing API key"
+            )
+        self.client = ZhipuAI(api_key=self.api_key)
 
     def pre_processing(self, **kwargs):
         supported_params = [
-            "model", "messages", "max_tokens", "temperature", "top_p", "n",
+            "model", "messages", "max_tokens", "temperature", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
         ]
         for key in list(kwargs.keys()):
             if key not in supported_params:
                 kwargs.pop(key)
         return kwargs
 
-    def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
-        result = self.client.chat.completions.create(
-            model=model, messages=messages, **new_kwargs
-        )
-        return self.response_model.post_stream_processing(result)
+    def post_stream_processing_wrapper(self, response):
+        return self.post_stream_processing(response)
 
     def create_model_response_wrapper(self, result, model):
-        # 调用 response_model 中的 create_model_response 方法
-        return self.response_model.create_model_response(result, model=model)
+        return self.create_model_response(result, model=model)
 
     def completion(self, model: str, messages: list, **kwargs):
         try:
             if model is None or messages is None:
-                raise LiteLLMOpenAIError(
+                raise ZhiPuOpenAIError(
                     status_code=422, message=f"Missing model or messages"
                 )
             new_kwargs = self.pre_processing(**kwargs)
-            stream = kwargs.get("stream", False)
+            stream = new_kwargs.get("stream", False)
 
             if stream:
-                return self.post_stream_processing_wrapper(model=model, messages=messages, **new_kwargs)
+                response = self.client.chat.completions.create(
+                    model=model, messages=messages, **new_kwargs
+                )
+                return self.post_stream_processing_wrapper(response)
             else:
-                result = completion(
+                result = self.client.chat.completions.create(
                     model=model, messages=messages, **new_kwargs
                 )
                 return self.create_model_response_wrapper(result, model=model)
         except Exception as e:
             if hasattr(e, "status_code"):
-                raise LiteLLMOpenAIError(status_code=e.status_code, message=str(e))
+                raise ZhiPuOpenAIError(status_code=e.status_code, message=str(e))
             else:
-                raise LiteLLMOpenAIError(status_code=500, message=str(e))
+                raise ZhiPuOpenAIError(status_code=500, message=str(e))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `unionllm-0.1.0/unionllm/providers/minimax.py` & `unionllm-0.1.1/unionllm/providers/minimax.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from .base_provider import BaseProvider
 from unionllm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
 import requests
 import json
-import logging
+import logging, os
 
 class MinimaxOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
 class MinimaxAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.api_key = model_kwargs.get("api_key")
+        # Get MINIMAX_API_KEY from environment variables
+        _env_api_key = os.environ.get("MINIMAX_API_KEY")
+        self.api_key = model_kwargs.get("api_key") if model_kwargs.get("api_key") else _env_api_key
+        if not self.api_key:
+            raise MinimaxOpenAIError(
+                status_code=422, message=f"Missing API key"
+            )
         self.endpoint_url = "https://api.minimax.chat/v1/text/chatcompletion_v2"
 
     def pre_processing(self, **kwargs):
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
@@ -101,14 +107,15 @@
                 raise MinimaxOpenAIError(
                     status_code=422, message=f"Missing model or messages"
                 )
             new_kwargs = self.pre_processing(**kwargs)
             stream = kwargs.get("stream", False)
 
             if stream:
+                print("streaming")
                 return self.post_stream_processing_wrapper(model=model, messages=messages, **new_kwargs)
             
             else:
                 payload = json.dumps({"model": model, "messages": messages, **new_kwargs})
                 headers = {
                     "Authorization": f"Bearer {self.api_key}",
                     "Content-Type": "application/json",
```

### Comparing `unionllm-0.1.0/unionllm/providers/moonshot.py` & `unionllm-0.1.1/unionllm/providers/moonshot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-import json
 from .base_provider import BaseProvider
-from unionllm.utils import ResponseModelInterface
 from openai import OpenAI
-import logging, json
+import logging, json, os
 
 
 class MoonshotOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
@@ -14,21 +12,26 @@
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
 
 class MoonshotAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.api_key = model_kwargs.get("api_key")
+        # Get MOONSHOT_API_KEY from environment variables
+        _env_api_key = os.environ.get("MOONSHOT_API_KEY")
+        self.api_key = model_kwargs.get("api_key") if model_kwargs.get("api_key") else _env_api_key
+        if not self.api_key:
+            raise MoonshotOpenAIError(
+                status_code=422, message=f"Missing API key"
+            )
         self.base_url = "https://api.moonshot.cn/v1"
-        self.response_model = ResponseModelInterface()
         self.client = OpenAI(api_key=self.api_key, base_url=self.base_url)
 
     def pre_processing(self, **kwargs):
-        # 处理参数兼容性问题，不支持的参数全部舍弃
+        # process the compatibility issue of parameters, all unsupported parameters are discarded
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
         ]
         for key in list(kwargs.keys()):
             if key not in supported_params:
@@ -36,19 +39,19 @@
 
         return kwargs
     
     def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
         result = self.client.chat.completions.create(
             model=model, messages=messages, **new_kwargs
         )
-        return self.response_model.post_stream_processing(result)
+        return self.post_stream_processing(result)
 
     def create_model_response_wrapper(self, result, model):
         # 调用 response_model 中的 create_model_response 方法
-        return self.response_model.create_model_response(result, model=model)
+        return self.create_model_response(result, model=model)
 
     def completion(self, model: str, messages: list, **kwargs):
         try:
             if model is None or messages is None:
                 raise MoonshotOpenAIError(
                     status_code=422, message=f"Missing model or messages"
                 )
```

### Comparing `unionllm-0.1.0/unionllm/providers/qwen.py` & `unionllm-0.1.1/unionllm/providers/qwen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-import json, time
 import dashscope
 from .base_provider import BaseProvider
 from http import HTTPStatus
 from dashscope import Generation
 from unionllm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
+import json, time, os
 
 class QwenOpenAIError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
 class QwenAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.api_key = model_kwargs.get("api_key")
+        # Get DASHSCOPE_API_KEY from environment variables
+        _env_api_key = os.environ.get("DASHSCOPE_API_KEY")
+        self.api_key = model_kwargs.get("api_key") if model_kwargs.get("api_key") else _env_api_key
+        if not self.api_key:
+            raise QwenOpenAIError(
+                status_code=422, message=f"Missing API key"
+            )        
         dashscope.api_key = self.api_key
 
     def pre_processing(self, **kwargs):
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
```

### Comparing `unionllm-0.1.0/unionllm/providers/tiangong.py` & `unionllm-0.1.1/unionllm/providers/tiangong.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import time
+import time, os
 import requests
 import json
 import hashlib
 from .base_provider import BaseProvider
 from unionllm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
 
 class TianGongOpenAIError(Exception):
@@ -13,16 +13,23 @@
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
 class TianGongAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.app_key = model_kwargs.get("app_key")
-        self.app_secret = model_kwargs.get("app_secret")
+        # Get TIANGONG_API_KEY from environment variables
+        _env_app_key = os.environ.get("TIANGONG_APP_KEY")
+        _env_app_secret = os.environ.get("TIANGONG_APP_SECRET")
+        self.app_key = model_kwargs.get("app_key") if model_kwargs.get("app_key") else _env_app_key
+        self.app_secret = model_kwargs.get("app_key") if model_kwargs.get("app_key") else _env_app_secret
+        if not self.app_key or not self.app_secret:
+            raise TianGongOpenAIError(
+                status_code=422, message=f"Missing APP key or APP secret"
+            )
         self.endpoint_url = "https://sky-api.singularity-ai.com/saas/api/v4/generate"
 
     def pre_processing(self, **kwargs):
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
```

### Comparing `unionllm-0.1.0/unionllm/providers/wenxin.py` & `unionllm-0.1.1/unionllm/providers/wenxin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import requests
-import json
+import json, os
 import logging
 import hashlib
 from .base_provider import BaseProvider
 from unionllm.utils import ModelResponse, Message, Choices, Usage, Delta, StreamingChoices
 
 class WenXinOpenAIError(Exception):
     def __init__(
@@ -14,16 +14,23 @@
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
 class WenXinAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.client_id = model_kwargs.get("client_id")
-        self.client_secret = model_kwargs.get("client_secret")
+        # Get ERNIE_CLIENT_ID and ERNIE_CLIENT_ID from environment variables
+        _env_client_id = os.environ.get("ERNIE_CLIENT_ID")
+        _env_client_secret = os.environ.get("ERNIE_CLIENT_SECRET")
+        self.client_id = model_kwargs.get("client_id") if model_kwargs.get("client_id") else _env_client_id
+        self.client_secret = model_kwargs.get("client_secret") if model_kwargs.get("client_secret") else _env_client_secret
+        if not self.client_id or not self.client_secret:
+            raise WenXinOpenAIError(
+                status_code=422, message=f"Missing client_id or client_secret"
+            )
         self.access_token = self.get_access_token()
 
     def get_access_token(self):
         url = "https://aip.baidubce.com/oauth/2.0/token"
         params = {
             "grant_type": "client_credentials",
             "client_id": self.client_id,
@@ -55,16 +62,14 @@
         index = 0
         for line in requests.post(self.endpoint_url, headers=headers, data=payload, stream=True).iter_lines():
             if line:
                 try:
                     # Remove the "data: " prefix before decoding the JSON
                     line_without_prefix = line.decode('utf-8').removeprefix('data: ')
                     new_line = json.loads(line_without_prefix)
-                    print(new_line)
-
                     chunk_choices = []
                     chunk_delta = Delta()
                     if new_line.get("result"):
                         chunk_delta.role = "assistant"
                         chunk_delta.content=new_line.get("result", "")
                         chunk_choices.append(StreamingChoices(index=index, delta=chunk_delta))
                     if 'usage' in new_line:
```

### Comparing `unionllm-0.1.0/unionllm/providers/xunfei.py` & `unionllm-0.1.1/unionllm/providers/xunfei.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .base_provider import BaseProvider
 from urllib.parse import urlparse
 import websocket
-import time
+import time, os
 import json
 import ssl
 import threading
 import logging
 import hmac
 import hashlib
 import base64
@@ -48,23 +48,22 @@
 
         signature_sha_base64 = base64.b64encode(signature_sha).decode(encoding='utf-8')
 
         authorization_origin = f'api_key="{self.APIKey}", algorithm="hmac-sha256", headers="host date request-line", signature="{signature_sha_base64}"'
 
         authorization = base64.b64encode(authorization_origin.encode('utf-8')).decode(encoding='utf-8')
 
-        # 将请求的鉴权参数组合为字典
+        # Make the request's authentication parameters into a dictionary
         v = {
             "authorization": authorization,
             "date": date,
             "host": self.host
         }
-        # 拼接鉴权参数，生成url
+        # Generate the final request URL
         url = self.Spark_url + '?' + urlencode(v)
-        # 此处打印出建立连接时候的url,参考本demo的时候可取消上方打印的注释，比对相同参数时生成的url与自己代码生成的url是否一致
         return url
 
 class XunfeiWebSocketClient:
     def __init__(self, app_id, api_key, api_secret, model, **kwargs):
         self.app_id = app_id
         self.api_key = api_key
         self.api_secret = api_secret
@@ -94,33 +93,28 @@
         try:
             data = json.loads(message)
             if data['header']['code'] == 0:
                 choices = data["payload"]["choices"]
                 for choice in choices["text"]:
                     self.answer += choice["content"]
                 
-                # 当会话结束（status=2）时处理usage信息
-                if data['header']['status'] == 2:  # 会话结束
+                if data['header']['status'] == 2:
                     if "usage" in data["payload"]:
                         usage = data["payload"]["usage"]
-                        # 假设usage信息中包含text字段，其中有prompt_tokens和completion_tokens
                         if "text" in usage:
                             text_usage = usage["text"]
-                            # 更新prompt_tokens和completion_tokens
                             self.prompt_tokens = text_usage.get("prompt_tokens", 0)
                             self.completion_tokens = text_usage.get("completion_tokens", 0)
                     
                     self.complete_event.set()
             else:
-                print(f"请求错误: {data['header']['code']}, {data['header']['message']}")
                 self.complete_event.set()
                 self.error = "connection error"
-                raise ValueError(f"请求错误: {data['header']['code']}, {data['header']['message']}")
+                raise ValueError(f"Request error: {data['header']['code']}, {data['header']['message']}")
         except json.JSONDecodeError as e:
-            print(f"JSON解析错误: {e}")
             self.error = e
             self.complete_event.set()
 
     def on_error(self, ws, error):
         logging.error(f"WebSocket error: {error}")
         self.error = error
         self.complete_event.set()
@@ -163,30 +157,38 @@
         self.complete_event.wait()  # 等待消息接收完成或出错
         wst.join()  # 确保WebSocket线程已结束
         return self.answer, {"prompt_tokens": self.prompt_tokens, "completion_tokens": self.completion_tokens}, self.error
 
 
 class XunfeiAIProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.app_id = model_kwargs.get("app_id")
-        self.api_key = model_kwargs.get("api_key")
-        self.api_secret = model_kwargs.get("api_secret")
+        # Get XUNFEI_APP_ID, XUNFEI_API_KEY, XUNFEI_API_SECRET from environment variables
+        _env_app_id = os.environ.get("XUNFEI_APP_ID")
+        _env_api_key = os.environ.get("XUNFEI_API_KEY")
+        _env_api_secret = os.environ.get("XUNFEI_API_SECRET")
+        
+        self.app_id = model_kwargs.get("app_id") if model_kwargs.get("app_id") else _env_app_id
+        self.api_key = model_kwargs.get("api_key") if model_kwargs.get("api_key") else _env_api_key
+        self.api_secret = model_kwargs.get("api_secret") if model_kwargs.get("api_secret") else _env_api_secret
+        if not self.app_id or not self.app_id or not self.api_secret:
+            raise XunfeiOpenAIError(
+                status_code=422, message=f"Missing app_id, api_key or api_secret"
+            )
 
     def pre_processing(self, **kwargs):
         if "app_id" in kwargs:
             self.app_id = kwargs.get("app_id")
             kwargs.pop("app_id")
         if "api_key" in kwargs:
             self.api_key = kwargs.get("api_key")
             kwargs.pop("api_key")
         if "api_secret" in kwargs:
             self.api_secret = kwargs.get("api_secret")
             kwargs.pop("api_secret")
 
-        # 处理参数兼容性问题，不支持的参数全部舍弃
         supported_params = [
             "model", "messages", "max_tokens", "temperature", "top_p", "top_k", 
         ]
         for key in list(kwargs.keys()):
             if key not in supported_params:
                 kwargs.pop(key)
```

### Comparing `unionllm-0.1.0/unionllm/providers/zhipu.py` & `unionllm-0.1.1/unionllm/providers/litellm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,60 @@
-import json
+import json, time
+import dashscope
 from .base_provider import BaseProvider
-from unionllm.utils import ResponseModelInterface
-from zhipuai import ZhipuAI
-import logging
+from litellm import completion
 
-class ZhiPuOpenAIError(Exception):
+class LiteLLMError(Exception):
     def __init__(
         self,
         status_code,
         message,
     ):
         self.status_code = status_code
         self.message = message
         super().__init__(self.message)
 
-class ZhipuAIProvider(BaseProvider):
+class LiteLLMProvider(BaseProvider):
     def __init__(self, **model_kwargs):
-        self.api_key = model_kwargs.get("api_key")
-        self.response_model = ResponseModelInterface()
-        self.client = ZhipuAI(api_key=self.api_key)
+        pass
 
     def pre_processing(self, **kwargs):
         supported_params = [
-            "model", "messages", "max_tokens", "temperature", "n",
+            "model", "messages", "max_tokens", "temperature", "top_p", "n",
             "logprobs", "stream", "stop", "presence_penalty", "frequency_penalty",
             "best_of", "logit_bias"
         ]
         for key in list(kwargs.keys()):
             if key not in supported_params:
                 kwargs.pop(key)
         return kwargs
 
-    def post_stream_processing_wrapper(self, response):
-        return self.response_model.post_stream_processing(response)
+    def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
+        result = completion(
+            model=model, messages=messages, **new_kwargs
+        )
+        return self.post_stream_processing(result)
 
     def create_model_response_wrapper(self, result, model):
-        return self.response_model.create_model_response(result, model=model)
+        return self.create_model_response(result, model=model)
 
     def completion(self, model: str, messages: list, **kwargs):
         try:
             if model is None or messages is None:
-                raise ZhiPuOpenAIError(
+                raise LiteLLMError(
                     status_code=422, message=f"Missing model or messages"
                 )
             new_kwargs = self.pre_processing(**kwargs)
-            stream = new_kwargs.get("stream", False)
+            stream = kwargs.get("stream", False)
 
             if stream:
-                response = self.client.chat.completions.create(
-                    model=model, messages=messages, **new_kwargs
-                )
-                return self.post_stream_processing_wrapper(response)
+                return self.post_stream_processing_wrapper(model=model, messages=messages, **new_kwargs)
             else:
-                result = self.client.chat.completions.create(
+                result = completion(
                     model=model, messages=messages, **new_kwargs
                 )
                 return self.create_model_response_wrapper(result, model=model)
         except Exception as e:
             if hasattr(e, "status_code"):
-                raise ZhiPuOpenAIError(status_code=e.status_code, message=str(e))
+                raise LiteLLMError(status_code=e.status_code, message=str(e))
             else:
-                raise ZhiPuOpenAIError(status_code=500, message=str(e))
+                raise LiteLLMError(status_code=500, message=str(e))
```

### Comparing `unionllm-0.1.0/unionllm/utils.py` & `unionllm-0.1.1/unionllm/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,14 @@
 from abc import ABC, abstractmethod
 from openai import OpenAIError as OriginalError
 from typing import List, Union, Optional
 
 import uuid, time, openai, random, requests
 from openai._models import BaseModel as OpenAIObject
 
-# from .exceptions import (
-#     AuthenticationError,
-#     BadRequestError,
-#     RateLimitError,
-#     ServiceUnavailableError,
-#     OpenAIError,
-#     ContextWindowExceededError,
-#     Timeout,
-#     APIConnectionError,
-#     APIError,
-#     BudgetExceededError
-# )
-
 class Message(OpenAIObject):
     def __init__(
         self,
         content="default",
         role="assistant",
         logprobs=None,
         function_call=None,
@@ -278,126 +265,125 @@
         # Allow dictionary-style access to attributes
         return getattr(self, key)
 
     def __setitem__(self, key, value):
         # Allow dictionary-style assignment of attributes
         setattr(self, key, value)
 
-class ResponseModelInterface:
-    def post_stream_processing(self, response, model=None):
-        for chunk in response:
-            print("chunk: ", chunk)
-            data = chunk.json()
-            if isinstance(data, str):
-                data = json.loads(data)
-            if 'choices' in data:
-                choices = data['choices']
-                chunk_choices = []
-                for choice in choices:
-                    delta = choice.get("delta")
-                    if delta:
-                        chunk_delta = Delta()
-                        if "role" in choice['delta']:
-                            chunk_delta.role = choice['delta']["role"]
-                        if "content" in choice['delta']:
-                            chunk_delta.content = choice['delta']["content"]
-                        chunk_choices.append(StreamingChoices(index=choice['index'], delta=chunk_delta))
-
-            if "usage" in data:
-                chunk_usage = Usage()
-                if data["usage"]:
-                    if "prompt_tokens" in data["usage"]:
-                        chunk_usage.prompt_tokens = data["usage"]["prompt_tokens"]
-                    if "completion_tokens" in data["usage"]:
-                        chunk_usage.completion_tokens = data["usage"]["completion_tokens"]
-                    if "total_tokens" in data["usage"]:
-                        chunk_usage.total_tokens = data["usage"]["total_tokens"]
+# class ResponseModelInterface:
+#     def post_stream_processing(self, response, model=None):
+#         for chunk in response:
+#             data = chunk.json()
+#             if isinstance(data, str):
+#                 data = json.loads(data)
+#             if 'choices' in data:
+#                 choices = data['choices']
+#                 chunk_choices = []
+#                 for choice in choices:
+#                     delta = choice.get("delta")
+#                     if delta:
+#                         chunk_delta = Delta()
+#                         if "role" in choice['delta']:
+#                             chunk_delta.role = choice['delta']["role"]
+#                         if "content" in choice['delta']:
+#                             chunk_delta.content = choice['delta']["content"]
+#                         chunk_choices.append(StreamingChoices(index=choice['index'], delta=chunk_delta))
+
+#             if "usage" in data:
+#                 chunk_usage = Usage()
+#                 if data["usage"]:
+#                     if "prompt_tokens" in data["usage"]:
+#                         chunk_usage.prompt_tokens = data["usage"]["prompt_tokens"]
+#                     if "completion_tokens" in data["usage"]:
+#                         chunk_usage.completion_tokens = data["usage"]["completion_tokens"]
+#                     if "total_tokens" in data["usage"]:
+#                         chunk_usage.total_tokens = data["usage"]["total_tokens"]
             
-            chunk_response = ModelResponse(
-                id=data["id"],
-                choices=chunk_choices,
-                created=data["created"],
-                model=model,
-                usage=chunk_usage if "usage" in data else None,
-                stream=True
-            )
-            yield chunk_response
-
-    def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
-        payload = json.dumps({"model": model, "messages": messages, **new_kwargs})
-        headers = {
-            "Authorization": f"Bearer {self.api_key}",
-            "Content-Type": "application/json",
-        }
-        response = requests.post(self.endpoint_url, headers=headers, data=payload)
-        for line in response.iter_lines():
-            print("line: ", line)
-            if line:
-                new_line = line.decode("utf-8").replace("data: ", "")
-                if new_line == "[DONE]":
-                    break
-                data = json.loads(new_line)
-                chunk_choices = []
-                for choice in data["choices"]:
-                    chunk_delta = Delta()
-                    delta = choice.get("delta")
-                    if delta:
-                        if "role" in choice['delta']:
-                            chunk_delta.role = choice['delta']["role"]
-                        if "content" in choice['delta']:
-                            chunk_delta.content = choice['delta']["content"]
-                        chunk_choices.append(StreamingChoices(index=choice['index'], delta=chunk_delta))
-
-                if "usage" in data:
-                    chunk_usage = Usage()
-                    if "prompt_tokens" in data["usage"]:
-                        chunk_usage.prompt_tokens = data["usage"]["prompt_tokens"]
-                    if "completion_tokens" in data["usage"]:
-                        chunk_usage.completion_tokens = data["usage"]["completion_tokens"]
-                    if "total_tokens" in data["usage"]:
-                        chunk_usage.total_tokens = data["usage"]["total_tokens"]
+#             chunk_response = ModelResponse(
+#                 id=data["id"],
+#                 choices=chunk_choices,
+#                 created=data["created"],
+#                 model=model,
+#                 usage=chunk_usage if "usage" in data else None,
+#                 stream=True
+#             )
+#             yield chunk_response
+
+#     def post_stream_processing_wrapper(self, model, messages, **new_kwargs):
+#         payload = json.dumps({"model": model, "messages": messages, **new_kwargs})
+#         headers = {
+#             "Authorization": f"Bearer {self.api_key}",
+#             "Content-Type": "application/json",
+#         }
+#         response = requests.post(self.endpoint_url, headers=headers, data=payload)
+#         for line in response.iter_lines():
+#             print("line: ", line)
+#             if line:
+#                 new_line = line.decode("utf-8").replace("data: ", "")
+#                 if new_line == "[DONE]":
+#                     break
+#                 data = json.loads(new_line)
+#                 chunk_choices = []
+#                 for choice in data["choices"]:
+#                     chunk_delta = Delta()
+#                     delta = choice.get("delta")
+#                     if delta:
+#                         if "role" in choice['delta']:
+#                             chunk_delta.role = choice['delta']["role"]
+#                         if "content" in choice['delta']:
+#                             chunk_delta.content = choice['delta']["content"]
+#                         chunk_choices.append(StreamingChoices(index=choice['index'], delta=chunk_delta))
+
+#                 if "usage" in data:
+#                     chunk_usage = Usage()
+#                     if "prompt_tokens" in data["usage"]:
+#                         chunk_usage.prompt_tokens = data["usage"]["prompt_tokens"]
+#                     if "completion_tokens" in data["usage"]:
+#                         chunk_usage.completion_tokens = data["usage"]["completion_tokens"]
+#                     if "total_tokens" in data["usage"]:
+#                         chunk_usage.total_tokens = data["usage"]["total_tokens"]
                 
-                chunk_response = ModelResponse(
-                    id=data["id"],
-                    choices=chunk_choices,
-                    created=data["created"],
-                    model=model,
-                    usage=chunk_usage if "usage" in data else None,
-                    stream=True
-                )
-                yield chunk_response
-
-
-    def create_model_response(
-        self, openai_response: openai.ChatCompletion, model: str
-    ) -> ModelResponse:
-        # print("openai_response: ", openai_response)
-        choices = []
-
-        for choice in openai_response.choices:
-            message = Message(content=choice.message.content, role=choice.message.role)
-            choices.append(
-                Choices(
-                    message=message, index=choice.index, finish_reason=choice.finish_reason
-                )
-            )
-
-        usage = Usage(
-            prompt_tokens=openai_response.usage.prompt_tokens,
-            completion_tokens=openai_response.usage.completion_tokens,
-            total_tokens=openai_response.usage.total_tokens,
-        )
-        response = ModelResponse(
-            id=openai_response.id,
-            choices=choices,
-            created=openai_response.created,
-            model=model,
-            usage=usage,
-        )
-        return response
+#                 chunk_response = ModelResponse(
+#                     id=data["id"],
+#                     choices=chunk_choices,
+#                     created=data["created"],
+#                     model=model,
+#                     usage=chunk_usage if "usage" in data else None,
+#                     stream=True
+#                 )
+#                 yield chunk_response
+
+
+#     def create_model_response(
+#         self, openai_response: openai.ChatCompletion, model: str
+#     ) -> ModelResponse:
+#         # print("openai_response: ", openai_response)
+#         choices = []
+
+#         for choice in openai_response.choices:
+#             message = Message(content=choice.message.content, role=choice.message.role)
+#             choices.append(
+#                 Choices(
+#                     message=message, index=choice.index, finish_reason=choice.finish_reason
+#                 )
+#             )
+
+#         usage = Usage(
+#             prompt_tokens=openai_response.usage.prompt_tokens,
+#             completion_tokens=openai_response.usage.completion_tokens,
+#             total_tokens=openai_response.usage.total_tokens,
+#         )
+#         response = ModelResponse(
+#             id=openai_response.id,
+#             choices=choices,
+#             created=openai_response.created,
+#             model=model,
+#             usage=usage,
+#         )
+#         return response
 
 class EmbeddingResponse(OpenAIObject):
     def __init__(
         self,
         id=None,
         choices=None,
         created=None,
```

