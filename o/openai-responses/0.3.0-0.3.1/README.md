# Comparing `tmp/openai_responses-0.3.0.tar.gz` & `tmp/openai_responses-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_responses-0.3.0.tar", max compression
+gzip compressed data, was "openai_responses-0.3.1.tar", max compression
```

## Comparing `openai_responses-0.3.0.tar` & `openai_responses-0.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1058 2024-03-20 02:09:50.213057 openai_responses-0.3.0/LICENSE
--rw-r--r--   0        0        0     3016 2024-05-14 18:14:24.699878 openai_responses-0.3.0/README.md
--rw-r--r--   0        0        0     1234 2024-05-13 17:16:29.612949 openai_responses-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      310 2024-05-03 15:30:48.556901 openai_responses-0.3.0/src/openai_responses/__init__.py
--rw-r--r--   0        0        0      606 2024-05-10 15:24:55.095526 openai_responses-0.3.0/src/openai_responses/_api.py
--rw-r--r--   0        0        0     1845 2024-05-14 15:18:04.142883 openai_responses-0.3.0/src/openai_responses/_mock.py
--rw-r--r--   0        0        0     3864 2024-05-13 15:32:42.633551 openai_responses-0.3.0/src/openai_responses/_routes/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-14 17:51:42.173434 openai_responses-0.3.0/src/openai_responses/_routes/_base.py
--rw-r--r--   0        0        0     6208 2024-05-10 14:26:39.440069 openai_responses-0.3.0/src/openai_responses/_routes/assistants.py
--rw-r--r--   0        0        0     1124 2024-05-13 15:47:22.432858 openai_responses-0.3.0/src/openai_responses/_routes/chat.py
--rw-r--r--   0        0        0     1386 2024-05-03 15:49:36.164682 openai_responses-0.3.0/src/openai_responses/_routes/embeddings.py
--rw-r--r--   0        0        0     4978 2024-05-03 18:04:28.339502 openai_responses-0.3.0/src/openai_responses/_routes/files.py
--rw-r--r--   0        0        0     8041 2024-05-10 14:28:24.653989 openai_responses-0.3.0/src/openai_responses/_routes/messages.py
--rw-r--r--   0        0        0     3767 2024-05-13 15:31:22.122002 openai_responses-0.3.0/src/openai_responses/_routes/run_steps.py
--rw-r--r--   0        0        0    11056 2024-05-10 19:13:45.175334 openai_responses-0.3.0/src/openai_responses/_routes/runs.py
--rw-r--r--   0        0        0     5335 2024-05-10 18:39:23.363809 openai_responses-0.3.0/src/openai_responses/_routes/threads.py
--rw-r--r--   0        0        0       62 2024-05-02 16:25:57.355893 openai_responses-0.3.0/src/openai_responses/_stores/__init__.py
--rw-r--r--   0        0        0     6059 2024-05-13 14:43:27.895252 openai_responses-0.3.0/src/openai_responses/_stores/state_store.py
--rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.3.0/src/openai_responses/_types/generics.py
--rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.3.0/src/openai_responses/_types/partials/assistants.py
--rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.3.0/src/openai_responses/_types/partials/chat.py
--rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.3.0/src/openai_responses/_types/partials/embeddings.py
--rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.3.0/src/openai_responses/_types/partials/files.py
--rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.3.0/src/openai_responses/_types/partials/messages.py
--rw-r--r--   0        0        0     2945 2024-05-13 15:43:24.432019 openai_responses-0.3.0/src/openai_responses/_types/partials/run_steps.py
--rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.3.0/src/openai_responses/_types/partials/runs.py
--rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.3.0/src/openai_responses/_types/partials/threads.py
--rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.3.0/src/openai_responses/_utils/copy.py
--rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.3.0/src/openai_responses/_utils/faker.py
--rw-r--r--   0        0        0      446 2024-05-03 15:46:30.517193 openai_responses-0.3.0/src/openai_responses/_utils/serde.py
--rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.3.0/src/openai_responses/_utils/time.py
--rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.3.0/src/openai_responses/helpers/builders/_base.py
--rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.3.0/src/openai_responses/helpers/builders/assistants.py
--rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.3.0/src/openai_responses/helpers/builders/chat.py
--rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.3.0/src/openai_responses/helpers/builders/embeddings.py
--rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.3.0/src/openai_responses/helpers/builders/messages.py
--rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.3.0/src/openai_responses/helpers/builders/run_steps.py
--rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.3.0/src/openai_responses/helpers/builders/runs.py
--rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.3.0/src/openai_responses/helpers/builders/threads.py
--rw-r--r--   0        0        0     1271 2024-05-13 15:42:07.751993 openai_responses-0.3.0/src/openai_responses/helpers/state_store.py
--rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.3.0/src/openai_responses/plugin.py
--rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.3.0/src/openai_responses/py.typed
--rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 openai_responses-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-16 18:41:10.309100 openai_responses-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3016 2024-05-14 18:14:24.699878 openai_responses-0.3.1/README.md
+-rw-r--r--   0        0        0     1234 2024-05-16 18:37:32.685674 openai_responses-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      310 2024-05-03 15:30:48.556901 openai_responses-0.3.1/src/openai_responses/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-10 15:24:55.095526 openai_responses-0.3.1/src/openai_responses/_api.py
+-rw-r--r--   0        0        0     1845 2024-05-14 15:18:04.142883 openai_responses-0.3.1/src/openai_responses/_mock.py
+-rw-r--r--   0        0        0     3864 2024-05-13 15:32:42.633551 openai_responses-0.3.1/src/openai_responses/_routes/__init__.py
+-rw-r--r--   0        0        0     5161 2024-05-14 17:51:42.173434 openai_responses-0.3.1/src/openai_responses/_routes/_base.py
+-rw-r--r--   0        0        0     6208 2024-05-16 18:36:55.630698 openai_responses-0.3.1/src/openai_responses/_routes/assistants.py
+-rw-r--r--   0        0        0     1123 2024-05-16 18:36:55.631029 openai_responses-0.3.1/src/openai_responses/_routes/chat.py
+-rw-r--r--   0        0        0     1385 2024-05-16 18:36:55.631618 openai_responses-0.3.1/src/openai_responses/_routes/embeddings.py
+-rw-r--r--   0        0        0     4978 2024-05-03 18:04:28.339502 openai_responses-0.3.1/src/openai_responses/_routes/files.py
+-rw-r--r--   0        0        0     8041 2024-05-16 18:36:55.631992 openai_responses-0.3.1/src/openai_responses/_routes/messages.py
+-rw-r--r--   0        0        0     3767 2024-05-13 15:31:22.122002 openai_responses-0.3.1/src/openai_responses/_routes/run_steps.py
+-rw-r--r--   0        0        0    11511 2024-05-16 18:36:55.632301 openai_responses-0.3.1/src/openai_responses/_routes/runs.py
+-rw-r--r--   0        0        0     5291 2024-05-16 18:36:55.632549 openai_responses-0.3.1/src/openai_responses/_routes/threads.py
+-rw-r--r--   0        0        0       62 2024-05-02 16:25:57.355893 openai_responses-0.3.1/src/openai_responses/_stores/__init__.py
+-rw-r--r--   0        0        0     6151 2024-05-16 18:37:01.157176 openai_responses-0.3.1/src/openai_responses/_stores/state_store.py
+-rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.3.1/src/openai_responses/_types/generics.py
+-rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.3.1/src/openai_responses/_types/partials/assistants.py
+-rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.3.1/src/openai_responses/_types/partials/chat.py
+-rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.3.1/src/openai_responses/_types/partials/embeddings.py
+-rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.3.1/src/openai_responses/_types/partials/files.py
+-rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.3.1/src/openai_responses/_types/partials/messages.py
+-rw-r--r--   0        0        0     2945 2024-05-13 15:43:24.432019 openai_responses-0.3.1/src/openai_responses/_types/partials/run_steps.py
+-rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.3.1/src/openai_responses/_types/partials/runs.py
+-rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.3.1/src/openai_responses/_types/partials/threads.py
+-rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.3.1/src/openai_responses/_utils/copy.py
+-rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.3.1/src/openai_responses/_utils/faker.py
+-rw-r--r--   0        0        0      627 2024-05-16 18:36:55.633057 openai_responses-0.3.1/src/openai_responses/_utils/serde.py
+-rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.3.1/src/openai_responses/_utils/time.py
+-rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.3.1/src/openai_responses/helpers/builders/_base.py
+-rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.3.1/src/openai_responses/helpers/builders/assistants.py
+-rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.3.1/src/openai_responses/helpers/builders/chat.py
+-rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.3.1/src/openai_responses/helpers/builders/embeddings.py
+-rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.3.1/src/openai_responses/helpers/builders/messages.py
+-rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.3.1/src/openai_responses/helpers/builders/run_steps.py
+-rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.3.1/src/openai_responses/helpers/builders/runs.py
+-rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.3.1/src/openai_responses/helpers/builders/threads.py
+-rw-r--r--   0        0        0     1271 2024-05-16 18:04:24.511337 openai_responses-0.3.1/src/openai_responses/helpers/state_store.py
+-rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.3.1/src/openai_responses/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.3.1/src/openai_responses/py.typed
+-rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 openai_responses-0.3.1/PKG-INFO
```

### Comparing `openai_responses-0.3.0/LICENSE` & `openai_responses-0.3.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -13,7 +13,8 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
```

### Comparing `openai_responses-0.3.0/README.md` & `openai_responses-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/pyproject.toml` & `openai_responses-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-responses"
-version = "0.3.0"
+version = "0.3.1"
 description = "Automatically mock OpenAI requests"
 authors = ["Michael Harris <mharris@definite.app>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mharrisb1/openai-responses-python"
 homepage = "https://mharrisb1.github.io/openai-responses-python/"
 documentation = "https://mharrisb1.github.io/openai-responses-python/"
```

### Comparing `openai_responses-0.3.0/src/openai_responses/_api.py` & `openai_responses-0.3.1/src/openai_responses/_api.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_mock.py` & `openai_responses-0.3.1/src/openai_responses/_mock.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/__init__.py` & `openai_responses-0.3.1/src/openai_responses/_routes/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/_base.py` & `openai_responses-0.3.1/src/openai_responses/_routes/_base.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/assistants.py` & `openai_responses-0.3.1/src/openai_responses/_routes/assistants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from typing import Any
 from typing_extensions import override
 
 import httpx
 import respx
 
 from openai.pagination import SyncCursorPage
@@ -16,15 +15,15 @@
 from .._types.partials.assistants import (
     PartialAssistant,
     PartialAssistantList,
     PartialAssistantDeleted,
 )
 
 from .._utils.faker import faker
-from .._utils.serde import model_dict, model_parse
+from .._utils.serde import json_loads, model_dict, model_parse
 from .._utils.time import utcnow_unix_timestamp_s
 
 __all__ = [
     "AssistantCreateRoute",
     "AssistantListRoute",
     "AssistantRetrieveRoute",
     "AssistantUpdateRoute",
@@ -48,15 +47,15 @@
         return httpx.Response(
             status_code=self._status_code,
             json=model_dict(model),
         )
 
     @staticmethod
     def _build(partial: PartialAssistant, request: httpx.Request) -> Assistant:
-        content = json.loads(request.content)
+        content = json_loads(request.content)
         defaults: PartialAssistant = {
             "id": faker.beta.assistant.id(),
             "created_at": utcnow_unix_timestamp_s(),
             "tools": [],
             "object": "assistant",
         }
         return model_parse(Assistant, defaults | partial | content)
@@ -148,15 +147,15 @@
     ) -> httpx.Response:
         self._route = route
         id = kwargs["id"]
         found = self._state.beta.assistants.get(id)
         if not found:
             return httpx.Response(404)
 
-        content: AssistantUpdateParams = json.loads(request.content)
+        content: AssistantUpdateParams = json_loads(request.content)
         deserialized = model_dict(found)
         updated = model_parse(Assistant, deserialized | content)
         self._state.beta.assistants.put(updated)
 
         return httpx.Response(status_code=200, json=model_dict(updated))
 
     @staticmethod
```

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/chat.py` & `openai_responses-0.3.1/src/openai_responses/_routes/chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-import json
-
 import httpx
 import respx
 
 from openai.types.chat.chat_completion import ChatCompletion
 
 from ._base import StatelessRoute
 
 from .._types.partials.chat import PartialChatCompletion
 
 from .._utils.faker import faker
-from .._utils.serde import model_parse
+from .._utils.serde import json_loads, model_parse
 from .._utils.time import utcnow_unix_timestamp_s
 
 __all__ = ["ChatCompletionsCreateRoute"]
 
 
 class ChatCompletionsCreateRoute(StatelessRoute[ChatCompletion, PartialChatCompletion]):
     def __init__(self, router: respx.MockRouter) -> None:
@@ -24,14 +22,14 @@
         )
 
     @staticmethod
     def _build(
         partial: PartialChatCompletion,
         request: httpx.Request,
     ) -> ChatCompletion:
-        content = json.loads(request.content)
+        content = json_loads(request.content)
         defaults: PartialChatCompletion = {
             "id": partial.get("id", faker.chat.completion.id()),
             "created": partial.get("created", utcnow_unix_timestamp_s()),
             "object": "chat.completion",
         }
         return model_parse(ChatCompletion, defaults | partial | content)
```

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/embeddings.py` & `openai_responses-0.3.1/src/openai_responses/_routes/embeddings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-import json
-
 from openai.types.embedding import Embedding
 from openai.types.embedding_create_params import EmbeddingCreateParams
 from openai.types.create_embedding_response import CreateEmbeddingResponse, Usage
 
 import httpx
 import respx
 
 from ._base import StatelessRoute
 
 from .._types.partials.embeddings import PartialCreateEmbeddingResponse
 
-from .._utils.serde import model_parse
+from .._utils.serde import json_loads, model_parse
 
 __all__ = ["EmbeddingsCreateRoute"]
 
 
 class EmbeddingsCreateRoute(
     StatelessRoute[
         CreateEmbeddingResponse,
@@ -29,15 +27,15 @@
         )
 
     @staticmethod
     def _build(
         partial: PartialCreateEmbeddingResponse,
         request: httpx.Request,
     ) -> CreateEmbeddingResponse:
-        content: EmbeddingCreateParams = json.loads(request.content)
+        content: EmbeddingCreateParams = json_loads(request.content)
         embeddings = partial.get("data", [])
         response = CreateEmbeddingResponse(
             data=[model_parse(Embedding, e) for e in embeddings],
             model=partial.get("model", content["model"]),
             object="list",
             usage=model_parse(
                 Usage,
```

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/files.py` & `openai_responses-0.3.1/src/openai_responses/_routes/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/messages.py` & `openai_responses-0.3.1/src/openai_responses/_routes/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from typing import Any
 from typing_extensions import override
 
 import httpx
 import respx
 
 from openai.pagination import SyncCursorPage
@@ -16,15 +15,15 @@
 from .._types.partials.messages import (
     PartialMessage,
     PartialMessageList,
     PartialMessageDeleted,
 )
 
 from .._utils.faker import faker
-from .._utils.serde import model_dict, model_parse
+from .._utils.serde import json_loads, model_dict, model_parse
 from .._utils.time import utcnow_unix_timestamp_s
 
 __all__ = [
     "MessageCreateRoute",
     "MessageListRoute",
     "MessageRetrieveRoute",
     "MessageUpdateRoute",
@@ -61,15 +60,15 @@
         return httpx.Response(
             status_code=self._status_code,
             json=model_dict(model),
         )
 
     @staticmethod
     def _build(partial: PartialMessage, request: httpx.Request) -> Message:
-        content = json.loads(request.content)
+        content = json_loads(request.content)
         defaults: PartialMessage = {
             "id": faker.beta.thread.message.id(),
             "content": [],
             "created_at": utcnow_unix_timestamp_s(),
             "object": "thread.message",
             "role": "user",
             "status": "completed",
@@ -205,15 +204,15 @@
             return httpx.Response(404)
 
         id = kwargs["id"]
         found_message = self._state.beta.threads.messages.get(id)
         if not found_message:
             return httpx.Response(404)
 
-        content: MessageUpdateParams = json.loads(request.content)
+        content: MessageUpdateParams = json_loads(request.content)
         deserialized = model_dict(found_message)
         updated = model_parse(Message, deserialized | content)
         self._state.beta.threads.messages.put(updated)
 
         return httpx.Response(status_code=200, json=model_dict(updated))
 
     @staticmethod
```

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/run_steps.py` & `openai_responses-0.3.1/src/openai_responses/_routes/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/runs.py` & `openai_responses-0.3.1/src/openai_responses/_routes/runs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 from openai.types.beta.threads.run import Run
 from openai.types.beta.threads.run_create_params import RunCreateParams
 from openai.types.beta.threads.run_update_params import RunUpdateParams
 from openai.types.beta.thread_create_and_run_params import ThreadCreateAndRunParams
 
 from ._base import StatefulRoute
 
+from ..helpers.builders.messages import message_from_create_request
 from ..helpers.builders.threads import thread_from_create_request
 
 from .._stores import StateStore
 from .._types.partials.runs import PartialRun, PartialRunList
 
 from .._utils.copy import model_copy
 from .._utils.faker import faker
-from .._utils.serde import model_dict, model_parse
+from .._utils.serde import json_loads, model_dict, model_parse
 from .._utils.time import utcnow_unix_timestamp_s
 
 
 __all__ = [
     "RunCreateRoute",
     "ThreadCreateAndRun",
     "RunListRoute",
@@ -55,15 +56,15 @@
         self._route = route
 
         thread_id = kwargs["thread_id"]
         found_thread = self._state.beta.threads.get(thread_id)
         if not found_thread:
             return httpx.Response(404)
 
-        content: RunCreateParams = json.loads(request.content)
+        content: RunCreateParams = json_loads(request.content)
 
         found_asst = self._state.beta.assistants.get(content["assistant_id"])
         if not found_asst:
             return httpx.Response(404)
 
         model = self._build(
             {
@@ -78,15 +79,15 @@
         return httpx.Response(
             status_code=self._status_code,
             json=model_dict(model),
         )
 
     @staticmethod
     def _build(partial: PartialRun, request: httpx.Request) -> Run:
-        content = json.loads(request.content)
+        content = json_loads(request.content)
         defaults: PartialRun = {
             "id": faker.beta.thread.run.id(),
             "created_at": utcnow_unix_timestamp_s(),
             "instructions": "",
             "object": "thread.run",
             "status": "queued",
         }
@@ -101,26 +102,32 @@
             state=state,
         )
 
     @override
     def _handler(self, request: httpx.Request, route: respx.Route) -> httpx.Response:
         self._route = route
 
-        content: ThreadCreateAndRunParams = json.loads(request.content)
+        content: ThreadCreateAndRunParams = json_loads(request.content)
 
         found_asst = self._state.beta.assistants.get(content["assistant_id"])
         if not found_asst:
             return httpx.Response(404)
 
         thread_create_params = content.get("thread", {})
         encoded = json.dumps(thread_create_params).encode("utf-8")
         thread_create_req = httpx.Request("", "", content=encoded)
         thread = thread_from_create_request(thread_create_req)
         self._state.beta.threads.put(thread)
 
+        for message_create_params in thread_create_params.get("messages", []):
+            encoded = json.dumps(message_create_params).encode("utf-8")
+            create_message_req = httpx.Request(method="", url="", content=encoded)
+            message = message_from_create_request(thread.id, create_message_req)
+            self._state.beta.threads.messages.put(message)
+
         model = self._build(
             {
                 "thread_id": thread.id,
                 "instructions": found_asst.instructions or "",
                 "model": found_asst.model,
                 "tools": [model_dict(t) for t in (found_asst.tools or [])],  # type: ignore
             },
@@ -130,15 +137,15 @@
         return httpx.Response(
             status_code=self._status_code,
             json=model_dict(model),
         )
 
     @staticmethod
     def _build(partial: PartialRun, request: httpx.Request) -> Run:
-        content = json.loads(request.content)
+        content = json_loads(request.content)
         if content.get("thread"):
             del content["thread"]
 
         return RunCreateRoute._build(partial, request)
 
 
 class RunListRoute(StatefulRoute[SyncCursorPage[Run], PartialRunList]):
@@ -256,15 +263,15 @@
             return httpx.Response(404)
 
         id = kwargs["id"]
         found_run = self._state.beta.threads.runs.get(id)
         if not found_run:
             return httpx.Response(404)
 
-        content: RunUpdateParams = json.loads(request.content)
+        content: RunUpdateParams = json_loads(request.content)
         deserialized = model_dict(found_run)
         updated = model_parse(Run, deserialized | content)
         self._state.beta.threads.runs.put(updated)
 
         return httpx.Response(status_code=200, json=model_dict(updated))
 
     @staticmethod
```

### Comparing `openai_responses-0.3.0/src/openai_responses/_routes/threads.py` & `openai_responses-0.3.1/src/openai_responses/_routes/threads.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from ..helpers.builders.messages import message_from_create_request
 
 from .._stores import StateStore
 from .._types.partials.threads import PartialThread, PartialThreadDeleted
 
 from .._utils.faker import faker
-from .._utils.serde import model_dict, model_parse
+from .._utils.serde import json_loads, model_dict, model_parse
 from .._utils.time import utcnow_unix_timestamp_s
 
 
 __all__ = [
     "ThreadCreateRoute",
     "ThreadRetrieveRoute",
     "ThreadUpdateRoute",
@@ -38,24 +38,23 @@
             state=state,
         )
 
     @override
     def _handler(self, request: httpx.Request, route: respx.Route) -> httpx.Response:
         self._route = route
 
-        content: ThreadCreateParams = json.loads(request.content)
+        content: ThreadCreateParams = json_loads(request.content)
         model = self._build({}, request)
         self._state.beta.threads.put(model)
 
-        if content.get("messages"):
-            for message_create_params in content.get("messages", []):
-                encoded = json.dumps(message_create_params).encode("utf-8")
-                create_message_req = httpx.Request(method="", url="", content=encoded)
-                message = message_from_create_request(model.id, create_message_req)
-                self._state.beta.threads.messages.put(message)
+        for message_create_params in content.get("messages", []):
+            encoded = json.dumps(message_create_params).encode("utf-8")
+            create_message_req = httpx.Request(method="", url="", content=encoded)
+            message = message_from_create_request(model.id, create_message_req)
+            self._state.beta.threads.messages.put(message)
 
         return httpx.Response(
             status_code=self._status_code,
             json=model_dict(model),
         )
 
     @staticmethod
```

### Comparing `openai_responses-0.3.0/src/openai_responses/_stores/state_store.py` & `openai_responses-0.3.1/src/openai_responses/_stores/state_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,19 +89,20 @@
             files = [file for file in files if file.purpose == purpose]
         return files
 
 
 class AssistantStore(BaseStore[Assistant]):
     def list(
         self,
-        limit: Optional[int] = None,
+        limit: Optional[str] = None,
         order: Optional[str] = None,
         after: Optional[str] = None,
         before: Optional[str] = None,
     ) -> List[Assistant]:
+        limit = limit or "20"
         objs = list(self._data.values())
         objs = list(reversed(objs)) if (order or "desc") == "desc" else objs
 
         start_ix = 0
         if after:
             obj = self._data.get(after)
             if obj:
@@ -110,34 +111,35 @@
         end_ix = None
         if before:
             obj = self._data.get(before)
             if obj:
                 end_ix = objs.index(obj)
 
         objs = objs[start_ix:end_ix]
-        return objs[: (limit or 20) + 1]
+        return objs[: int(limit)]
 
 
 class ThreadStore(BaseStore[Thread]):
     def __init__(self) -> None:
         super().__init__()
         self.messages = MessageStore()
         self.runs = RunStore()
 
 
 class MessageStore(BaseStore[Message]):
     def list(
         self,
         thread_id: str,
-        limit: Optional[int] = None,
+        limit: Optional[str] = None,
         order: Optional[str] = None,
         after: Optional[str] = None,
         before: Optional[str] = None,
         run_id: Optional[str] = None,
     ) -> List[Message]:
+        limit = limit or "20"
         objs = [m for m in list(self._data.values()) if m.thread_id == thread_id]
         if run_id:
             objs = [obj for obj in objs if obj.run_id == run_id]
         objs = list(reversed(objs)) if (order or "desc") == "desc" else objs
 
         start_ix = 0
         if after:
@@ -148,30 +150,31 @@
         end_ix = None
         if before:
             obj = self._data.get(before)
             if obj:
                 end_ix = objs.index(obj)
 
         objs = objs[start_ix:end_ix]
-        return objs[: (limit or 20) + 1]
+        return objs[: int(limit)]
 
 
 class RunStore(BaseStore[Run]):
     def __init__(self) -> None:
         super().__init__()
         self.steps = RunStepStore()
 
     def list(
         self,
         thread_id: str,
-        limit: Optional[int] = None,
+        limit: Optional[str] = None,
         order: Optional[str] = None,
         after: Optional[str] = None,
         before: Optional[str] = None,
     ) -> List[Run]:
+        limit = limit or "20"
         objs = [m for m in list(self._data.values()) if m.thread_id == thread_id]
         objs = list(reversed(objs)) if (order or "desc") == "desc" else objs
 
         start_ix = 0
         if after:
             obj = self._data.get(after)
             if obj:
@@ -180,27 +183,28 @@
         end_ix = None
         if before:
             obj = self._data.get(before)
             if obj:
                 end_ix = objs.index(obj)
 
         objs = objs[start_ix:end_ix]
-        return objs[: (limit or 20) + 1]
+        return objs[: int(limit)]
 
 
 class RunStepStore(BaseStore[RunStep]):
     def list(
         self,
         thread_id: str,
         run_id: str,
-        limit: Optional[int] = None,
+        limit: Optional[str] = None,
         order: Optional[str] = None,
         after: Optional[str] = None,
         before: Optional[str] = None,
     ) -> List[RunStep]:
+        limit = limit or "20"
         objs = [
             m
             for m in list(self._data.values())
             if m.thread_id == thread_id and m.run_id == run_id
         ]
         objs = list(reversed(objs)) if (order or "desc") == "desc" else objs
 
@@ -213,8 +217,8 @@
         end_ix = None
         if before:
             obj = self._data.get(before)
             if obj:
                 end_ix = objs.index(obj)
 
         objs = objs[start_ix:end_ix]
-        return objs[: (limit or 20) + 1]
+        return objs[: int(limit)]
```

### Comparing `openai_responses-0.3.0/src/openai_responses/_types/partials/assistants.py` & `openai_responses-0.3.1/src/openai_responses/_types/partials/assistants.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_types/partials/chat.py` & `openai_responses-0.3.1/src/openai_responses/_types/partials/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_types/partials/embeddings.py` & `openai_responses-0.3.1/src/openai_responses/_types/partials/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_types/partials/files.py` & `openai_responses-0.3.1/src/openai_responses/_types/partials/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_types/partials/messages.py` & `openai_responses-0.3.1/src/openai_responses/_types/partials/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_types/partials/run_steps.py` & `openai_responses-0.3.1/src/openai_responses/_types/partials/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_types/partials/runs.py` & `openai_responses-0.3.1/src/openai_responses/_types/partials/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/_types/partials/threads.py` & `openai_responses-0.3.1/src/openai_responses/_types/partials/threads.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/helpers/builders/chat.py` & `openai_responses-0.3.1/src/openai_responses/helpers/builders/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/helpers/builders/embeddings.py` & `openai_responses-0.3.1/src/openai_responses/helpers/builders/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/helpers/builders/messages.py` & `openai_responses-0.3.1/src/openai_responses/helpers/builders/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/helpers/builders/run_steps.py` & `openai_responses-0.3.1/src/openai_responses/helpers/builders/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/helpers/builders/runs.py` & `openai_responses-0.3.1/src/openai_responses/helpers/builders/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/src/openai_responses/helpers/state_store.py` & `openai_responses-0.3.1/src/openai_responses/helpers/state_store.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.0/PKG-INFO` & `openai_responses-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-responses
-Version: 0.3.0
+Version: 0.3.1
 Summary: Automatically mock OpenAI requests
 Home-page: https://mharrisb1.github.io/openai-responses-python/
 License: MIT
 Author: Michael Harris
 Author-email: mharris@definite.app
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

