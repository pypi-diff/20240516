# Comparing `tmp/wagtail_ai-2.0.1.tar.gz` & `tmp/wagtail_ai-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_ai-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wagtail_ai-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtail_ai-2.0.1.tar` & `wagtail_ai-2.1.0.tar`

### file list

```diff
@@ -1,31 +1,35 @@
--rw-r--r--   0        0        0     1067 2024-01-19 14:35:55.740987 wagtail_ai-2.0.1/LICENSE
--rw-r--r--   0        0        0     1186 2024-01-19 14:35:55.740987 wagtail_ai-2.0.1/LICENSE_LANGCHAIN
--rw-r--r--   0        0        0     2089 2024-01-19 14:35:55.740987 wagtail_ai-2.0.1/README.md
--rw-r--r--   0        0        0      560 2024-01-19 14:35:55.740987 wagtail_ai-2.0.1/SECURITY.md
--rw-r--r--   0        0        0     2368 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      497 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/setup.cfg
--rw-r--r--   0        0        0      122 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/__init__.py
--rw-r--r--   0        0        0     5766 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/ai/__init__.py
--rw-r--r--   0        0        0     3455 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/ai/base.py
--rw-r--r--   0        0        0     2550 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/ai/echo.py
--rw-r--r--   0        0        0     1996 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/ai/llm.py
--rw-r--r--   0        0        0      154 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/apps.py
--rw-r--r--   0        0        0     1161 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/forms.py
--rw-r--r--   0        0        0     2147 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/migrations/0001_initial.py
--rw-r--r--   0        0        0     1163 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/migrations/0002_populate_default_prompts.py
--rw-r--r--   0        0        0        0 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/migrations/__init__.py
--rw-r--r--   0        0        0     2501 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/models.py
--rw-r--r--   0        0        0     1397 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/prompts.py
--rw-r--r--   0        0        0     1577 2024-01-19 14:36:07.016826 wagtail_ai-2.0.1/src/wagtail_ai/static/wagtail_ai/main.css
--rw-r--r--   0        0        0    11170 2024-01-19 14:36:07.016826 wagtail_ai-2.0.1/src/wagtail_ai/static/wagtail_ai/wagtail-ai.js
--rw-r--r--   0        0        0        0 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/text_splitters/__init__.py
--rw-r--r--   0        0        0      583 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/text_splitters/dummy.py
--rw-r--r--   0        0        0     6673 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/text_splitters/langchain.py
--rw-r--r--   0        0        0     1707 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/text_splitters/length.py
--rw-r--r--   0        0        0      529 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/tokens.py
--rw-r--r--   0        0        0      614 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/types.py
--rw-r--r--   0        0        0        0 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/utils/__init__.py
--rw-r--r--   0        0        0      172 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/utils/deprecation.py
--rw-r--r--   0        0        0     4719 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/views.py
--rw-r--r--   0        0        0     2504 2024-01-19 14:35:55.744987 wagtail_ai-2.0.1/src/wagtail_ai/wagtail_hooks.py
--rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 wagtail_ai-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-16 10:17:14.889112 wagtail_ai-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1186 2024-05-16 10:17:14.889112 wagtail_ai-2.1.0/LICENSE_LANGCHAIN
+-rw-r--r--   0        0        0     2631 2024-05-16 10:17:14.889112 wagtail_ai-2.1.0/README.md
+-rw-r--r--   0        0        0      560 2024-05-16 10:17:14.889112 wagtail_ai-2.1.0/SECURITY.md
+-rw-r--r--   0        0        0     2368 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      497 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/setup.cfg
+-rw-r--r--   0        0        0      122 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/__init__.py
+-rw-r--r--   0        0        0     6351 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/ai/__init__.py
+-rw-r--r--   0        0        0     3825 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/ai/base.py
+-rw-r--r--   0        0        0     2822 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/ai/echo.py
+-rw-r--r--   0        0        0     1996 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/ai/llm.py
+-rw-r--r--   0        0        0     4047 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/ai/openai.py
+-rw-r--r--   0        0        0      208 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/apps.py
+-rw-r--r--   0        0        0     2060 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/forms.py
+-rw-r--r--   0        0        0     2147 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1163 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/migrations/0002_populate_default_prompts.py
+-rw-r--r--   0        0        0        0 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/migrations/__init__.py
+-rw-r--r--   0        0        0     2501 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/models.py
+-rw-r--r--   0        0        0     1397 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/prompts.py
+-rw-r--r--   0        0        0     1577 2024-05-16 10:17:23.861209 wagtail_ai-2.1.0/src/wagtail_ai/static/wagtail_ai/draftail.css
+-rw-r--r--   0        0        0    12873 2024-05-16 10:17:23.861209 wagtail_ai-2.1.0/src/wagtail_ai/static/wagtail_ai/draftail.js
+-rw-r--r--   0        0        0     2106 2024-05-16 10:17:23.861209 wagtail_ai-2.1.0/src/wagtail_ai/static/wagtail_ai/image_description.css
+-rw-r--r--   0        0        0     7818 2024-05-16 10:17:23.861209 wagtail_ai-2.1.0/src/wagtail_ai/static/wagtail_ai/image_description.js
+-rw-r--r--   0        0        0      205 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/templates/wagtail_ai/widgets/image_title.html
+-rw-r--r--   0        0        0        0 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/text_splitters/__init__.py
+-rw-r--r--   0        0        0      591 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/text_splitters/dummy.py
+-rw-r--r--   0        0        0     6673 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/text_splitters/langchain.py
+-rw-r--r--   0        0        0     1707 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/text_splitters/length.py
+-rw-r--r--   0        0        0      529 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/tokens.py
+-rw-r--r--   0        0        0      614 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/types.py
+-rw-r--r--   0        0        0        0 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/utils/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/utils/deprecation.py
+-rw-r--r--   0        0        0     7103 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/views.py
+-rw-r--r--   0        0        0     2708 2024-05-16 10:17:14.893112 wagtail_ai-2.1.0/src/wagtail_ai/wagtail_hooks.py
+-rw-r--r--   0        0        0     4271 1970-01-01 00:00:00.000000 wagtail_ai-2.1.0/PKG-INFO
```

### Comparing `wagtail_ai-2.0.1/LICENSE` & `wagtail_ai-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/LICENSE_LANGCHAIN` & `wagtail_ai-2.1.0/LICENSE_LANGCHAIN`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/README.md` & `wagtail_ai-2.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,27 +11,52 @@
 Wagtail AI integrates Wagtail with AI's APIs (think ChatGPT) to help you write and correct your content.
 
 Right now, it can:
 
 * Finish what you've started - write some text and tell Wagtail AI to finish it off for you
 * Correct your spelling/grammar
 * Let you add your own custom prompts
+* Automatically generate alt-tags for your uploaded images
 * Work with multiple LLM providers including local models, OpenAI, Mistral, Claude and many others
 
+## Demos
+
+### Rich-text integration
+
 https://user-images.githubusercontent.com/27112/223072938-8cb5ccff-4835-489a-8be4-cca85001885e.mp4
 
+### Alt-text generation
+
+https://github.com/wagtail/wagtail-ai/assets/27617/5ffd5493-b39c-4d38-bed8-fdd243920eb5
+
 ## Requirements & Costs
 
-Wagtail AI supports [many different LLMs](https://wagtail-ai.readthedocs.io/latest/ai-backends/), with OpenAI models available by default.
+Wagtail AI supports [many different LLMs](https://wagtail-ai.readthedocs.io/latest/ai-backends/), with OpenAI models
+available by default. To use these, you'll need an OpenAI account and an API key. There'll also be some cost involved.
+
+For the OpenAI API used here (`gpt-3.5-turbo`), the [cost](https://openai.com/pricing) is
+
+- $0.0005 per 1000 tokens for input tokens (prompt)
+- $0.0015 per 1000 tokens for output tokens (answer)
+
+Here is an estimated cost breakdown for the `correction` prompt on a 1000-word paragraph.
+
+### We assume that:
+
+- Prompt is 30 words and the existing paragraph is 1000 words (Input)
+- Each word is 1.3 tokens (Tokens multiplier)
+- We get back 1000 words back (Output)
 
-To use these, you'll need an OpenAI account and an API key. There'll also be some cost involved. For the OpenAI API used here, OpenAI charges $0.002 for 1,000 tokens (a word is about 1.3 tokens). Every token sent to the API, and every token we get back counts, so you can expect using 'correction' on 1,000 word paragraph to cost roughly:
+### Then:
 
-* (1,000 * 1.3) + (35 * 1.3) (for the initial prompt) tokens sent to the API
-* \+ (1,000 * 1.3) tokens received from the API
-* = 2,645 tokens = $0.0053
+- **Input tokens :** (35 + 1000) x 1.3 = 1345.5 tokens.
+- **Output tokens :** 1000 x 1.3 = 1300
+- **Input tokens cost :** 1345.5 / 1000 * $0.0005 = $0.00067275
+- **Output tokens cost :** 1300 / 1000 * $0.0015 = $0.00195
+- **Total cost :** $0.00262275
 
 ## Links
 
 - [Documentation](https://wagtail-ai.readthedocs.io/)
 - [Changelog](https://github.com/wagtail/wagtail-ai/blob/main/CHANGELOG.md)
 - [Contributing](https://wagtail-ai.readthedocs.io/latest/contributing/)
 - [Discussions](https://github.com/wagtail/wagtail-ai/discussions)
```

### Comparing `wagtail_ai-2.0.1/SECURITY.md` & `wagtail_ai-2.1.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/pyproject.toml` & `wagtail_ai-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/ai/__init__.py` & `wagtail_ai-2.1.0/src/wagtail_ai/ai/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.module_loading import import_string
 
 from ..text_splitters.langchain import LangchainRecursiveCharacterTextSplitter
 from ..text_splitters.length import NaiveTextSplitterCalculator
 from ..types import TextSplitterLengthCalculatorProtocol, TextSplitterProtocol
 from ..utils import deprecation
-from .base import AIBackend, BaseAIBackendConfigSettings
+from .base import AIBackend, BackendFeature, BaseAIBackendConfigSettings
 
 
 class TextSplittingSettingsDict(TypedDict):
     SPLITTER_CLASS: NotRequired[str]
     SPLITTER_LENGTH_CALCULATOR_CLASS: NotRequired[str]
 
 
@@ -157,7 +157,26 @@
     config = ai_backend_cls.config_cls.from_settings(
         backend_settings,
         text_splitter_class=text_splitting.splitter_class,
         text_splitter_length_calculator_class=text_splitting.splitter_length_calculator_class,
     )
 
     return ai_backend_cls(config=config)
+
+
+class BackendNotFound(Exception):
+    pass
+
+
+def get_backend(feature: BackendFeature = BackendFeature.TEXT_COMPLETION) -> AIBackend:
+    match feature:
+        case BackendFeature.TEXT_COMPLETION:
+            alias = settings.WAGTAIL_AI.get("TEXT_COMPLETION_BACKEND", "default")
+        case BackendFeature.IMAGE_DESCRIPTION:
+            alias = settings.WAGTAIL_AI.get("IMAGE_DESCRIPTION_BACKEND")
+        case _:
+            alias = None
+
+    if alias is None:
+        raise BackendNotFound(f"No backend found for {feature.name}")
+
+    return get_ai_backend(alias)
```

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/ai/base.py` & `wagtail_ai-2.1.0/src/wagtail_ai/ai/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,38 @@
-from abc import ABCMeta, abstractmethod
+from abc import ABCMeta
 from dataclasses import dataclass
+from enum import Enum
 from typing import (
     Any,
     ClassVar,
     Generic,
     NotRequired,
     Protocol,
     Required,
     Self,
     TypedDict,
     TypeVar,
 )
 
 from django.core.exceptions import ImproperlyConfigured
+from django.core.files import File
 
 from .. import tokens
 from ..types import (
     AIResponse,
     TextSplitterLengthCalculatorProtocol,
     TextSplitterProtocol,
 )
 
 
+class BackendFeature(Enum):
+    TEXT_COMPLETION = "TEXT_COMPLETION"
+    IMAGE_DESCRIPTION = "IMAGE_DESCRIPTION"
+
+
 class BaseAIBackendConfigSettings(TypedDict):
     MODEL_ID: Required[str]
     TOKEN_LIMIT: NotRequired[int | None]
 
 
 AIBackendConfigSettings = TypeVar(
     "AIBackendConfigSettings", bound=BaseAIBackendConfigSettings, contravariant=True
@@ -95,24 +102,26 @@
     def __init__(
         self,
         *,
         config: AIBackendConfig,
     ) -> None:
         self.config = config
 
-    @abstractmethod
     def prompt_with_context(
         self, *, pre_prompt: str, context: str, post_prompt: str | None = None
     ) -> AIResponse:
         """
         Given a prompt and a context, return a response.
         """
-        ...
+        raise NotImplementedError("This backend does not support text completion")
 
     def get_text_splitter(self) -> TextSplitterProtocol:
         return self.config.text_splitter_class(
             chunk_size=self.config.token_limit,
             length_function=self.get_splitter_length_calculator().get_splitter_length,
         )
 
     def get_splitter_length_calculator(self) -> TextSplitterLengthCalculatorProtocol:
         return self.config.text_splitter_length_calculator_class()
+
+    def describe_image(self, *, image_file: File, prompt: str) -> AIResponse:
+        raise NotImplementedError("This backend does not support image description")
```

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/ai/echo.py` & `wagtail_ai-2.1.0/src/wagtail_ai/ai/echo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
 import time
 from collections.abc import Generator, Iterator
 from dataclasses import dataclass
 from typing import Any, NotRequired, Self
 
 from django.core.exceptions import ImproperlyConfigured
+from django.core.files import File
 
 from .base import (
     AIBackend,
     AIResponse,
     BaseAIBackendConfig,
     BaseAIBackendConfigSettings,
 )
@@ -58,18 +59,26 @@
 
 class EchoBackend(AIBackend[EchoBackendConfig]):
     config_cls = EchoBackendConfig
 
     def prompt_with_context(
         self, *, pre_prompt: str, context: str, post_prompt: str | None = None
     ) -> AIResponse:
+        return self.get_response(
+            ["This", "is", "an", "echo", "backend:", *context.split()]
+        )
+
+    def describe_image(self, *, image_file: File, prompt: str) -> AIResponse:
+        return self.get_response(
+            ["This", "is", "an", "echo", "backend:", image_file.name]
+        )
+
+    def get_response(self, words):
         def response_iterator() -> Generator[str, None, None]:
-            response = ["This", "is", "an", "echo", "backend:"]
-            response += context.split()
-            for word in response:
+            for word in words:
                 if (
                     self.config.max_word_sleep_seconds is not None
                     and self.config.max_word_sleep_seconds > 0
                 ):
                     time.sleep(
                         random.random()
                         * random.randint(0, self.config.max_word_sleep_seconds)
```

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/ai/llm.py` & `wagtail_ai-2.1.0/src/wagtail_ai/ai/llm.py`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/migrations/0001_initial.py` & `wagtail_ai-2.1.0/src/wagtail_ai/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/migrations/0002_populate_default_prompts.py` & `wagtail_ai-2.1.0/src/wagtail_ai/migrations/0002_populate_default_prompts.py`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/models.py` & `wagtail_ai-2.1.0/src/wagtail_ai/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/prompts.py` & `wagtail_ai-2.1.0/src/wagtail_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/static/wagtail_ai/main.css` & `wagtail_ai-2.1.0/src/wagtail_ai/static/wagtail_ai/draftail.css`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/static/wagtail_ai/wagtail-ai.js` & `wagtail_ai-2.1.0/src/wagtail_ai/static/wagtail_ai/draftail.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,174 @@
 (() => {
     "use strict";
     var e = {
-            733: (e, t, n) => {
+            499: (e, t, n) => {
                 n.r(t)
             },
-            883: function(e, t, n) {
+            557: function(e, t) {
+                var n, r = this && this.__extends || (n = function(e, t) {
+                        return n = Object.setPrototypeOf || {
+                            __proto__: []
+                        }
+                        instanceof Array && function(e, t) {
+                            e.__proto__ = t
+                        } || function(e, t) {
+                            for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
+                        }, n(e, t)
+                    }, function(e, t) {
+                        if ("function" != typeof t && null !== t) throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
+
+                        function r() {
+                            this.constructor = e
+                        }
+                        n(e, t), e.prototype = null === t ? Object.create(t) : (r.prototype = t.prototype, new r)
+                    }),
+                    o = this && this.__awaiter || function(e, t, n, r) {
+                        return new(n || (n = Promise))((function(o, a) {
+                            function i(e) {
+                                try {
+                                    l(r.next(e))
+                                } catch (e) {
+                                    a(e)
+                                }
+                            }
+
+                            function u(e) {
+                                try {
+                                    l(r.throw(e))
+                                } catch (e) {
+                                    a(e)
+                                }
+                            }
+
+                            function l(e) {
+                                var t;
+                                e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
+                                    e(t)
+                                }))).then(i, u)
+                            }
+                            l((r = r.apply(e, t || [])).next())
+                        }))
+                    },
+                    a = this && this.__generator || function(e, t) {
+                        var n, r, o, a, i = {
+                            label: 0,
+                            sent: function() {
+                                if (1 & o[0]) throw o[1];
+                                return o[1]
+                            },
+                            trys: [],
+                            ops: []
+                        };
+                        return a = {
+                            next: u(0),
+                            throw: u(1),
+                            return: u(2)
+                        }, "function" == typeof Symbol && (a[Symbol.iterator] = function() {
+                            return this
+                        }), a;
+
+                        function u(u) {
+                            return function(l) {
+                                return function(u) {
+                                    if (n) throw new TypeError("Generator is already executing.");
+                                    for (; a && (a = 0, u[0] && (i = 0)), i;) try {
+                                        if (n = 1, r && (o = 2 & u[0] ? r.return : u[0] ? r.throw || ((o = r.return) && o.call(r), 0) : r.next) && !(o = o.call(r, u[1])).done) return o;
+                                        switch (r = 0, o && (u = [2 & u[0], o.value]), u[0]) {
+                                            case 0:
+                                            case 1:
+                                                o = u;
+                                                break;
+                                            case 4:
+                                                return i.label++, {
+                                                    value: u[1],
+                                                    done: !1
+                                                };
+                                            case 5:
+                                                i.label++, r = u[1], u = [0];
+                                                continue;
+                                            case 7:
+                                                u = i.ops.pop(), i.trys.pop();
+                                                continue;
+                                            default:
+                                                if (!((o = (o = i.trys).length > 0 && o[o.length - 1]) || 6 !== u[0] && 2 !== u[0])) {
+                                                    i = 0;
+                                                    continue
+                                                }
+                                                if (3 === u[0] && (!o || u[1] > o[0] && u[1] < o[3])) {
+                                                    i.label = u[1];
+                                                    break
+                                                }
+                                                if (6 === u[0] && i.label < o[1]) {
+                                                    i.label = o[1], o = u;
+                                                    break
+                                                }
+                                                if (o && i.label < o[2]) {
+                                                    i.label = o[2], i.ops.push(u);
+                                                    break
+                                                }
+                                                o[2] && i.ops.pop(), i.trys.pop();
+                                                continue
+                                        }
+                                        u = t.call(e, i)
+                                    } catch (e) {
+                                        u = [6, e], r = 0
+                                    } finally {
+                                        n = o = 0
+                                    }
+                                    if (5 & u[0]) throw u[1];
+                                    return {
+                                        value: u[0] ? u[1] : void 0,
+                                        done: !0
+                                    }
+                                }([u, l])
+                            }
+                        }
+                    };
+                t.__esModule = !0, t.fetchResponse = t.getAIConfiguration = void 0;
+                var i = function(e) {
+                    function t() {
+                        return null !== e && e.apply(this, arguments) || this
+                    }
+                    return r(t, e), t
+                }(Error);
+                t.getAIConfiguration = function() {
+                    var e = document.querySelector("#wagtail-ai-config");
+                    if (!e || !e.textContent) throw new Error("No wagtail-ai configuration found.");
+                    try {
+                        return JSON.parse(e.textContent)
+                    } catch (e) {
+                        throw new SyntaxError("Error parsing wagtail-ai configuration: ".concat(e.message))
+                    }
+                }, t.fetchResponse = function(e, n, r) {
+                    return o(void 0, void 0, void 0, (function() {
+                        var o, u, l, c;
+                        return a(this, (function(a) {
+                            switch (a.label) {
+                                case 0:
+                                    return a.trys.push([0, 3, , 4]), o = (0, t.getAIConfiguration)().urls, [4, fetch(o[e], {
+                                        method: "POST",
+                                        body: n,
+                                        signal: r
+                                    })];
+                                case 1:
+                                    return [4, (u = a.sent()).json()];
+                                case 2:
+                                    if (l = a.sent(), u.ok) return [2, l.message];
+                                    throw new i(l.error);
+                                case 3:
+                                    throw c = a.sent(), new i(c.message);
+                                case 4:
+                                    return [2]
+                            }
+                        }))
+                    }))
+                }
+            },
+            394: function(e, t, n) {
                 var r = this && this.__createBinding || (Object.create ? function(e, t, n, r) {
                         void 0 === r && (r = n);
                         var o = Object.getOwnPropertyDescriptor(t, n);
                         o && !("get" in o ? !t.__esModule : o.writable || o.configurable) || (o = {
                             enumerable: !0,
                             get: function() {
                                 return t[n]
@@ -139,22 +299,23 @@
                             default: e
                         }
                     };
                 t.__esModule = !0;
                 var c = a(n(363)),
                     s = n(3),
                     f = n(533),
-                    d = n(324),
-                    p = l(n(724)),
-                    h = n(843),
-                    v = ["Processing your query, please wait...", "Analyzing your input, just a moment...", "Generating a response, hold on...", "Thinking, thinking, thinking...", "Fetching data, almost there...", "Compiling information, please wait...", "Crunching numbers, please be patient...", "Analyzing data, loading...", "Preparing response, please wait...", "Interpreting your message, loading..."];
+                    d = n(166),
+                    p = l(n(272)),
+                    h = n(851),
+                    v = n(557),
+                    y = ["Processing your query, please wait...", "Analyzing your input, just a moment...", "Generating a response, hold on...", "Thinking, thinking, thinking...", "Fetching data, almost there...", "Compiling information, please wait...", "Crunching numbers, please be patient...", "Analyzing data, loading...", "Preparing response, please wait...", "Interpreting your message, loading..."];
 
                 function g(e) {
                     var t = e.cancelHandler,
-                        n = v[Math.floor(Math.random() * v.length)];
+                        n = y[Math.floor(Math.random() * y.length)];
                     return c.default.createElement("div", {
                         className: "Draftail-AI-LoadingOverlay"
                     }, c.default.createElement("span", null, c.default.createElement("svg", {
                         className: "icon icon-spinner c-spinner",
                         "aria-hidden": "true"
                     }, c.default.createElement("use", {
                         href: "#icon-spinner"
@@ -181,84 +342,84 @@
                         }, c.default.createElement("span", null, e.label), " ", e.description)
                     })))
                 }
                 t.default = function(e) {
                     var t = this,
                         n = e.getEditorState,
                         r = e.onChange,
-                        o = (0, h.getAIConfiguration)().aiPrompts,
+                        o = (0, v.getAIConfiguration)().aiPrompts,
                         a = n(),
                         l = (0, c.useState)(!1),
                         d = l[0],
-                        v = l[1],
-                        y = (0, c.useState)(!1),
-                        b = y[0],
-                        w = y[1],
-                        _ = (0, c.useState)(null),
-                        E = _[0],
-                        S = _[1],
-                        x = (0, c.useRef)(),
-                        A = (null == x ? void 0 : x.current) ? null == x ? void 0 : x.current.closest("[data-draftail-editor-wrapper]") : null,
-                        M = new AbortController;
+                        y = l[1],
+                        b = (0, c.useState)(!1),
+                        w = b[0],
+                        _ = b[1],
+                        E = (0, c.useState)(null),
+                        x = E[0],
+                        S = E[1],
+                        A = (0, c.useRef)(),
+                        M = (null == A ? void 0 : A.current) ? null == A ? void 0 : A.current.closest("[data-draftail-editor-wrapper]") : null,
+                        O = new AbortController;
                     return c.default.createElement(c.default.Fragment, null, c.default.createElement(s.ToolbarButton, {
                         name: "AI Tools",
                         title: "AI prompts",
                         icon: p.default,
                         onClick: function() {
-                            return w(!b)
+                            return _(!w)
                         }
                     }), c.default.createElement("span", {
-                        ref: x
-                    }), b ? c.default.createElement(m, {
+                        ref: A
+                    }), w ? c.default.createElement(m, {
                         close: function() {
-                            return w(!1)
+                            return _(!1)
                         },
                         onAction: function(e) {
                             return i(t, void 0, void 0, (function() {
                                 var t, n, o;
                                 return u(this, (function(i) {
                                     switch (i.label) {
                                         case 0:
-                                            S(null), w(!1), v(!0), i.label = 1;
+                                            S(null), _(!1), y(!0), i.label = 1;
                                         case 1:
-                                            return i.trys.push([1, 6, , 7]), "append" !== e.method ? [3, 3] : (t = r, [4, (0, h.processAction)(a, e, h.handleAppend, M)]);
+                                            return i.trys.push([1, 6, , 7]), "append" !== e.method ? [3, 3] : (t = r, [4, (0, h.processAction)(a, e, h.handleAppend, O)]);
                                         case 2:
                                             return t.apply(void 0, [i.sent()]), [3, 5];
                                         case 3:
-                                            return n = r, [4, (0, h.processAction)(a, e, h.handleReplace, M)];
+                                            return n = r, [4, (0, h.processAction)(a, e, h.handleReplace, O)];
                                         case 4:
                                             n.apply(void 0, [i.sent()]), i.label = 5;
                                         case 5:
                                             return [3, 7];
                                         case 6:
                                             return o = i.sent(), S(o.message), [3, 7];
                                         case 7:
-                                            return v(!1), [2]
+                                            return y(!1), [2]
                                     }
                                 }))
                             }))
                         },
                         aiPrompts: o
-                    }) : null, E && (null == A ? void 0 : A.parentNode) ? (0, f.createPortal)(c.default.createElement("div", {
+                    }) : null, x && (null == M ? void 0 : M.parentNode) ? (0, f.createPortal)(c.default.createElement("div", {
                         className: "w-field__errors"
                     }, c.default.createElement("svg", {
                         className: "icon icon-warning w-field__errors-icon",
                         "aria-hidden": "true"
                     }, c.default.createElement("use", {
                         href: "#icon-warning"
                     })), " ", c.default.createElement("p", {
                         className: "error-message"
-                    }, E)), A.parentNode.previousElementSibling) : null, d && A ? (0, f.createPortal)(c.default.createElement(g, {
+                    }, x)), M.parentNode.previousElementSibling) : null, d && M ? (0, f.createPortal)(c.default.createElement(g, {
                         cancelHandler: function(e) {
-                            e.preventDefault(), M.abort(), v(!1)
+                            e.preventDefault(), O.abort(), y(!1)
                         }
-                    }), A) : null)
+                    }), M) : null)
                 }
             },
-            724: function(e, t, n) {
+            272: function(e, t, n) {
                 var r = this && this.__importDefault || function(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 };
                 t.__esModule = !0;
                 var o = r(n(363)),
@@ -274,61 +435,44 @@
                             }, o.default.createElement("path", {
                                 d: "M234.7 42.7L197 56.8c-3 1.1-5 4-5 7.2s2 6.1 5 7.2l37.7 14.1L248.8 123c1.1 3 4 5 7.2 5s6.1-2 7.2-5l14.1-37.7L315 71.2c3-1.1 5-4 5-7.2s-2-6.1-5-7.2L277.3 42.7 263.2 5c-1.1-3-4-5-7.2-5s-6.1 2-7.2 5L234.7 42.7zM46.1 395.4c-18.7 18.7-18.7 49.1 0 67.9l34.6 34.6c18.7 18.7 49.1 18.7 67.9 0L529.9 116.5c18.7-18.7 18.7-49.1 0-67.9L495.3 14.1c-18.7-18.7-49.1-18.7-67.9 0L46.1 395.4zM484.6 82.6l-105 105-23.3-23.3 105-105 23.3 23.3zM7.5 117.2C3 118.9 0 123.2 0 128s3 9.1 7.5 10.8L64 160l21.2 56.5c1.7 4.5 6 7.5 10.8 7.5s9.1-3 10.8-7.5L128 160l56.5-21.2c4.5-1.7 7.5-6 7.5-10.8s-3-9.1-7.5-10.8L128 96 106.8 39.5C105.1 35 100.8 32 96 32s-9.1 3-10.8 7.5L64 96 7.5 117.2zm352 256c-4.5 1.7-7.5 6-7.5 10.8s3 9.1 7.5 10.8L416 416l21.2 56.5c1.7 4.5 6 7.5 10.8 7.5s9.1-3 10.8-7.5L480 416l56.5-21.2c4.5-1.7 7.5-6 7.5-10.8s-3-9.1-7.5-10.8L480 352l-21.2-56.5c-1.7-4.5-6-7.5-10.8-7.5s-9.1 3-10.8 7.5L416 352l-56.5 21.2z"
                             }))
                         }), null)
                     });
                 t.default = i
             },
-            324: (e, t, n) => {
+            166: (e, t, n) => {
                 t.__esModule = !0, t.useOutsideAlerter = void 0;
                 var r = n(363);
                 t.useOutsideAlerter = function(e, t) {
                     var n = (0, r.useRef)((function(n) {
                         e.current && !e.current.contains(n.target) && t()
                     }));
                     (0, r.useEffect)((function() {
                         return document.addEventListener("mousedown", n.current),
                             function() {
                                 document.removeEventListener("mousedown", n.current)
                             }
                     }), [n])
                 }
             },
-            75: function(e, t, n) {
+            569: function(e, t, n) {
                 var r = this && this.__importDefault || function(e) {
                     return e && e.__esModule ? e : {
                         default: e
                     }
                 };
-                t.__esModule = !0, n(733);
-                var o = r(n(883));
+                t.__esModule = !0, n(499);
+                var o = r(n(394));
                 window.draftail.registerPlugin({
                     type: "ai",
                     inline: o.default
                 }, "controls")
             },
-            843: function(e, t, n) {
-                var r, o = this && this.__extends || (r = function(e, t) {
-                        return r = Object.setPrototypeOf || {
-                            __proto__: []
-                        }
-                        instanceof Array && function(e, t) {
-                            e.__proto__ = t
-                        } || function(e, t) {
-                            for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
-                        }, r(e, t)
-                    }, function(e, t) {
-                        if ("function" != typeof t && null !== t) throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
-
-                        function n() {
-                            this.constructor = e
-                        }
-                        r(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
-                    }),
-                    a = this && this.__awaiter || function(e, t, n, r) {
+            851: function(e, t, n) {
+                var r = this && this.__awaiter || function(e, t, n, r) {
                         return new(n || (n = Promise))((function(o, a) {
                             function i(e) {
                                 try {
                                     l(r.next(e))
                                 } catch (e) {
                                     a(e)
                                 }
@@ -347,15 +491,15 @@
                                 e.done ? o(e.value) : (t = e.value, t instanceof n ? t : new n((function(e) {
                                     e(t)
                                 }))).then(i, u)
                             }
                             l((r = r.apply(e, t || [])).next())
                         }))
                     },
-                    i = this && this.__generator || function(e, t) {
+                    o = this && this.__generator || function(e, t) {
                         var n, r, o, a, i = {
                             label: 0,
                             sent: function() {
                                 if (1 & o[0]) throw o[1];
                                 return o[1]
                             },
                             trys: [],
@@ -422,83 +566,50 @@
                                         value: u[0] ? u[1] : void 0,
                                         done: !0
                                     }
                                 }([u, l])
                             }
                         }
                     };
-                t.__esModule = !0, t.processAction = t.handleReplace = t.handleAppend = t.getAIConfiguration = void 0;
-                var u = n(603),
-                    l = function(e) {
-                        function t() {
-                            return null !== e && e.apply(this, arguments) || this
-                        }
-                        return o(t, e), t
-                    }(Error);
-                t.getAIConfiguration = function() {
-                    var e = document.querySelector("#wagtail-ai-config");
-                    if (!e || !e.textContent) throw new Error("No wagtail-ai configuration found.");
-                    try {
-                        return JSON.parse(e.textContent)
-                    } catch (e) {
-                        throw new SyntaxError("Error parsing wagtail-ai configuration: ".concat(e.message))
-                    }
-                };
-                var c = function(e, n, r) {
-                    return a(void 0, void 0, void 0, (function() {
-                        var o, a, u, c, s;
-                        return i(this, (function(i) {
-                            switch (i.label) {
-                                case 0:
-                                    (o = new FormData).append("text", e), o.append("prompt", n.uuid), i.label = 1;
-                                case 1:
-                                    return i.trys.push([1, 4, , 5]), a = (0, t.getAIConfiguration)().aiProcessUrl, [4, fetch(a, {
-                                        method: "POST",
-                                        body: o,
-                                        signal: r
-                                    })];
-                                case 2:
-                                    return [4, (u = i.sent()).json()];
-                                case 3:
-                                    if (c = i.sent(), u.ok) return [2, c.message];
-                                    throw new l(c.error);
-                                case 4:
-                                    throw s = i.sent(), new l(s.message);
-                                case 5:
-                                    return [2]
-                            }
+                t.__esModule = !0, t.processAction = t.handleReplace = t.handleAppend = t.fetchAIResponse = void 0;
+                var a = n(603),
+                    i = n(557);
+                t.fetchAIResponse = function(e, t, n) {
+                    return r(void 0, void 0, void 0, (function() {
+                        var r;
+                        return o(this, (function(o) {
+                            return (r = new FormData).append("text", e), r.append("prompt", t.uuid), [2, (0, i.fetchResponse)("TEXT_COMPLETION", r, n)]
                         }))
                     }))
-                };
-                t.handleAppend = function(e, t) {
-                    var n = u.RichUtils.insertSoftNewline(u.EditorState.moveSelectionToEnd(e)),
+                }, t.handleAppend = function(e, t) {
+                    var n = a.RichUtils.insertSoftNewline(a.EditorState.moveSelectionToEnd(e)),
                         r = n.getCurrentContent(),
-                        o = u.Modifier.replaceText(r, u.EditorState.moveSelectionToEnd(n).getSelection(), t);
-                    return u.EditorState.push(n, o, "insert-characters")
+                        o = a.Modifier.replaceText(r, a.EditorState.moveSelectionToEnd(n).getSelection(), t);
+                    return a.EditorState.push(n, o, "insert-characters")
                 }, t.handleReplace = function(e, t) {
                     var n = e.getCurrentContent(),
-                        r = u.Modifier.replaceText(n, function(e) {
+                        r = a.Modifier.replaceText(n, function(e) {
                             var t = e.getBlockMap();
-                            return new u.SelectionState({
+                            return new a.SelectionState({
                                 anchorKey: t.first().getKey(),
                                 anchorOffset: 0,
                                 focusKey: t.last().getKey(),
                                 focusOffset: t.last().getLength()
                             })
                         }(n), t);
-                    return u.EditorState.push(e, r, "insert-characters")
-                }, t.processAction = function(e, t, n, r) {
-                    return a(void 0, void 0, void 0, (function() {
-                        var o, a, u;
-                        return i(this, (function(i) {
-                            switch (i.label) {
+                    return a.EditorState.push(e, r, "insert-characters")
+                }, t.processAction = function(e, n, a, i) {
+                    return r(void 0, void 0, void 0, (function() {
+                        var r, u, l;
+                        return o(this, (function(o) {
+                            switch (o.label) {
                                 case 0:
-                                    return o = e.getCurrentContent(), a = o.getPlainText(), [4, c(a, t, r.signal)];
+                                    return r = e.getCurrentContent(), u = r.getPlainText(), [4, (0, t.fetchAIResponse)(u, n, i.signal)];
                                 case 1:
-                                    return u = i.sent(), [2, n(e, u)]
+                                    return l = o.sent(), [2, a(e, l)]
                             }
                         }))
                     }))
                 }
             },
             603: e => {
                 e.exports = DraftJS
@@ -525,9 +636,9 @@
     }
     n.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, n(75)
+    }, n(569)
 })();
```

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/text_splitters/dummy.py` & `wagtail_ai-2.1.0/src/wagtail_ai/text_splitters/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class DummyTextSplitter(TextSplitterProtocol):
     def __init__(
         self, *, chunk_size: int, length_function: Callable[[str], int]
     ) -> None:
         pass
 
-    def split_text(self, text: str) -> str:
+    def split_text(self, text: str) -> list[str]:
         # Don't do any splitting.
-        return text
+        return [text]
 
 
 class DummyLengthCalculator(TextSplitterLengthCalculatorProtocol):
     def get_splitter_length(self, text: str) -> int:
         return len(text)
```

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/text_splitters/langchain.py` & `wagtail_ai-2.1.0/src/wagtail_ai/text_splitters/langchain.py`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/text_splitters/length.py` & `wagtail_ai-2.1.0/src/wagtail_ai/text_splitters/length.py`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/tokens.py` & `wagtail_ai-2.1.0/src/wagtail_ai/tokens.py`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/types.py` & `wagtail_ai-2.1.0/src/wagtail_ai/types.py`

 * *Files identical despite different names*

### Comparing `wagtail_ai-2.0.1/src/wagtail_ai/wagtail_hooks.py` & `wagtail_ai-2.1.0/src/wagtail_ai/wagtail_hooks.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,34 @@
 from django.utils.html import json_script
 from django.utils.safestring import mark_safe
 from django.views.i18n import JavaScriptCatalog
 from wagtail import hooks
 from wagtail.admin.rich_text.editors.draftail.features import ControlFeature
 
 from .models import Prompt
-from .views import process, prompt_viewset
+from .views import describe_image, prompt_viewset, text_completion
 
 
 @hooks.register("register_admin_urls")  # type: ignore
 def register_admin_urls():
     urls = [
         path(
             "jsi18n/",
             JavaScriptCatalog.as_view(packages=["wagtail_ai"]),
             name="javascript_catalog",
         ),
         path(
-            "process/",
-            process,
-            name="process",
+            "text_completion/",
+            text_completion,
+            name="text_completion",
+        ),
+        path(
+            "describe_image/",
+            describe_image,
+            name="describe_image",
         ),
     ]
 
     return [
         path(
             "ai/",
             include(
@@ -46,16 +51,16 @@
     features.register_editor_plugin(
         "draftail",
         feature_name,
         ControlFeature(
             {
                 "type": feature_name,
             },
-            js=["wagtail_ai/wagtail-ai.js"],
-            css={"all": ["wagtail_ai/main.css"]},
+            js=["wagtail_ai/draftail.js"],
+            css={"all": ["wagtail_ai/draftail.css"]},
         ),
     )
 
 
 class PromptDict(TypedDict):
     # Fields should match the Prompt type defined in custom.d.ts
     # be careful not to expose any sensitive or exploitable data here.
@@ -76,23 +81,23 @@
     }
 
 
 def get_prompts():
     return [_serialize_prompt(prompt) for prompt in Prompt.objects.all()]
 
 
-@hooks.register("insert_editor_js")  # type: ignore
+@hooks.register("insert_global_admin_js")  # type: ignore
 def ai_editor_js():
-    prompt_json = get_prompts()
-    process_url = reverse("wagtail_ai:process")
-
-    wagtail_ai_config = json_script(
-        {"aiPrompts": prompt_json, "aiProcessUrl": process_url},
-        "wagtail-ai-config",
-    )
+    config = {
+        "aiPrompts": get_prompts(),
+        "urls": {
+            "TEXT_COMPLETION": reverse("wagtail_ai:text_completion"),
+            "DESCRIBE_IMAGE": reverse("wagtail_ai:describe_image"),
+        },
+    }
 
-    return mark_safe(wagtail_ai_config)
+    return mark_safe(json_script(config, "wagtail-ai-config"))
 
 
 @hooks.register("register_admin_viewset")  # type: ignore
 def register_viewset():
     return prompt_viewset
```

### Comparing `wagtail_ai-2.0.1/PKG-INFO` & `wagtail_ai-2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-ai
-Version: 2.0.1
+Version: 2.1.0
 Summary: Get a hand writing your content with AI super powers!
 Author-email: Tom Usher <tom@tomusher.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -50,27 +50,52 @@
 Wagtail AI integrates Wagtail with AI's APIs (think ChatGPT) to help you write and correct your content.
 
 Right now, it can:
 
 * Finish what you've started - write some text and tell Wagtail AI to finish it off for you
 * Correct your spelling/grammar
 * Let you add your own custom prompts
+* Automatically generate alt-tags for your uploaded images
 * Work with multiple LLM providers including local models, OpenAI, Mistral, Claude and many others
 
+## Demos
+
+### Rich-text integration
+
 https://user-images.githubusercontent.com/27112/223072938-8cb5ccff-4835-489a-8be4-cca85001885e.mp4
 
+### Alt-text generation
+
+https://github.com/wagtail/wagtail-ai/assets/27617/5ffd5493-b39c-4d38-bed8-fdd243920eb5
+
 ## Requirements & Costs
 
-Wagtail AI supports [many different LLMs](https://wagtail-ai.readthedocs.io/latest/ai-backends/), with OpenAI models available by default.
+Wagtail AI supports [many different LLMs](https://wagtail-ai.readthedocs.io/latest/ai-backends/), with OpenAI models
+available by default. To use these, you'll need an OpenAI account and an API key. There'll also be some cost involved.
+
+For the OpenAI API used here (`gpt-3.5-turbo`), the [cost](https://openai.com/pricing) is
+
+- $0.0005 per 1000 tokens for input tokens (prompt)
+- $0.0015 per 1000 tokens for output tokens (answer)
+
+Here is an estimated cost breakdown for the `correction` prompt on a 1000-word paragraph.
+
+### We assume that:
+
+- Prompt is 30 words and the existing paragraph is 1000 words (Input)
+- Each word is 1.3 tokens (Tokens multiplier)
+- We get back 1000 words back (Output)
 
-To use these, you'll need an OpenAI account and an API key. There'll also be some cost involved. For the OpenAI API used here, OpenAI charges $0.002 for 1,000 tokens (a word is about 1.3 tokens). Every token sent to the API, and every token we get back counts, so you can expect using 'correction' on 1,000 word paragraph to cost roughly:
+### Then:
 
-* (1,000 * 1.3) + (35 * 1.3) (for the initial prompt) tokens sent to the API
-* \+ (1,000 * 1.3) tokens received from the API
-* = 2,645 tokens = $0.0053
+- **Input tokens :** (35 + 1000) x 1.3 = 1345.5 tokens.
+- **Output tokens :** 1000 x 1.3 = 1300
+- **Input tokens cost :** 1345.5 / 1000 * $0.0005 = $0.00067275
+- **Output tokens cost :** 1300 / 1000 * $0.0015 = $0.00195
+- **Total cost :** $0.00262275
 
 ## Links
 
 - [Documentation](https://wagtail-ai.readthedocs.io/)
 - [Changelog](https://github.com/wagtail/wagtail-ai/blob/main/CHANGELOG.md)
 - [Contributing](https://wagtail-ai.readthedocs.io/latest/contributing/)
 - [Discussions](https://github.com/wagtail/wagtail-ai/discussions)
```

