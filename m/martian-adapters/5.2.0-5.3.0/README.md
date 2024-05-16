# Comparing `tmp/martian_adapters-5.2.0.tar.gz` & `tmp/martian_adapters-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-5.2.0.tar", max compression
+gzip compressed data, was "martian_adapters-5.3.0.tar", max compression
```

## Comparing `martian_adapters-5.2.0.tar` & `martian_adapters-5.3.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0    35149 2024-05-15 00:48:05.227455 martian_adapters-5.2.0/LICENSE
--rw-r--r--   0        0        0     3623 2024-05-15 00:48:05.227455 martian_adapters-5.2.0/README.md
--rw-r--r--   0        0        0      725 2024-05-15 00:48:05.227455 martian_adapters-5.2.0/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-05-15 00:48:05.227455 martian_adapters-5.2.0/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2188 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     2125 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2486 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0      523 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5915 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     6154 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3352 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0     1017 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9067 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4020 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2498 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     3116 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7458 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1672 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     3032 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1593 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1167 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4280 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2536 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2438 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    11133 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/rate_limiter.py
--rw-r--r--   0        0        0      316 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/requirements.txt
--rw-r--r--   0        0        0     7067 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/types.py
--rw-r--r--   0        0        0        0 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1147 2024-05-15 00:48:05.231455 martian_adapters-5.2.0/pyproject.toml
--rw-r--r--   0        0        0     4924 1970-01-01 00:00:00.000000 martian_adapters-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/LICENSE
+-rw-r--r--   0        0        0     3623 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/README.md
+-rw-r--r--   0        0        0      725 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     2125 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2486 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0      523 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5915 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     6154 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3352 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0     1092 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9067 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4020 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     6077 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/provider_adapters/cohere_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2498 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3116 2024-05-16 19:41:28.949992 martian_adapters-5.3.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7458 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1672 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     3032 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1593 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1167 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4280 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2536 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2438 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    11133 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      316 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/requirements.txt
+-rw-r--r--   0        0        0     7067 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1165 2024-05-16 19:41:28.953992 martian_adapters-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4963 1970-01-01 00:00:00.000000 martian_adapters-5.3.0/PKG-INFO
```

### Comparing `martian_adapters-5.2.0/LICENSE` & `martian_adapters-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/README.md` & `martian_adapters-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/__init__.py` & `martian_adapters-5.3.0/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-5.3.0/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-5.3.0/adapters/abstract_adapters/base_adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Abstract base class for all LLM adapters.
     It defines the interface for creating subclasses and concrete adapters.
     Provides the structure to create a nesting of different adapters and LLM access
     """
 
     @abstractmethod
     def get_model(self) -> Model:
-        """Returns the martain model object, this is used to identify the model which is used by the adapter
+        """Returns the martian model object, this is used to identify the model which is used by the adapter
 
         Returns:
             # Model: model object
         """
 
     @abstractmethod
     async def execute_async(
```

### Comparing `martian_adapters-5.2.0/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-5.3.0/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-5.3.0/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-5.3.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-5.3.0/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-5.3.0/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/adapter_factory.py` & `martian_adapters-5.3.0/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-5.3.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/__init__.py` & `martian_adapters-5.3.0/adapters/provider_adapters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .anthropic_sdk_chat_provider_adapter import AnthropicSDKChatProviderAdapter
 from .anyscale_sdk_chat_provider_adapter import AnyscaleSDKChatProviderAdapter
+from .cohere_sdk_chat_provider_adapter import CohereSDKChatProviderAdapter
 from .deepinfra_sdk_chat_provider_adapter import DeepInfraSDKChatProviderAdapter
 from .fireworks_sdk_chat_provider_adapter import FireworksSDKChatProviderAdapter
 from .gemini_sdk_chat_provider_adapter import GeminiSDKChatProviderAdapter
 from .groq_sdk_chat_provider_adapter import GroqSDKChatProviderAdapter
 from .lepton_sdk_chat_provider_adapter import LeptonSDKChatProviderAdapter
 from .moonshot_sdk_chat_provider_adapter import MoonshotSDKChatProviderAdapter
 from .octoai_sdk_chat_provider_adapter import OctoaiSDKChatProviderAdapter
```

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/lepton_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-5.3.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/rate_limiter.py` & `martian_adapters-5.3.0/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/types.py` & `martian_adapters-5.3.0/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/utils/general_utils.py` & `martian_adapters-5.3.0/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/utils/network_utils.py` & `martian_adapters-5.3.0/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/adapters/utils/openai_client_factory.py` & `martian_adapters-5.3.0/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-5.2.0/pyproject.toml` & `martian_adapters-5.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "5.2.0"
+version = "5.3.0"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -27,14 +27,15 @@
 pydantic = "^2.4.2"
 together = "^0.2.6"
 transformers = "^4.36.0"
 sentencepiece = "^0.1.99"
 openai = "1.23.6"
 vcrpy = "^6.0.1"
 google-generativeai = "^0.3.2"
+cohere = "^5.3.4"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
 pytest-dotenv = "^0.5.2"
 pytest-asyncio = "^0.21.1"
 pytest-recording = "^0.13.1"
```

### Comparing `martian_adapters-5.2.0/PKG-INFO` & `martian_adapters-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 5.2.0
+Version: 5.3.0
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
 Requires-Dist: aiosignal (>=1.3.1,<2.0.0)
 Requires-Dist: anthropic (==0.16.0)
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
 Requires-Dist: charset-normalizer (>=3.2.0,<4.0.0)
+Requires-Dist: cohere (>=5.3.4,<6.0.0)
 Requires-Dist: frozenlist (>=1.4.0,<2.0.0)
 Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
 Requires-Dist: idna (>=3.7,<4.0)
 Requires-Dist: isort (>=5.12.0,<6.0.0)
 Requires-Dist: multidict (>=6.0.4,<7.0.0)
 Requires-Dist: openai (==1.23.6)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
```

