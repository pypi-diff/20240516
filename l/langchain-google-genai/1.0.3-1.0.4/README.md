# Comparing `tmp/langchain_google_genai-1.0.3.tar.gz` & `tmp/langchain_google_genai-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_genai-1.0.3.tar", max compression
+gzip compressed data, was "langchain_google_genai-1.0.4.tar", max compression
```

## Comparing `langchain_google_genai-1.0.3.tar` & `langchain_google_genai-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1072 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/LICENSE
--rw-r--r--   0        0        0     2875 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/README.md
--rw-r--r--   0        0        0     2762 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/langchain_google_genai/__init__.py
--rw-r--r--   0        0        0      136 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/langchain_google_genai/_common.py
--rw-r--r--   0        0        0      163 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/langchain_google_genai/_enums.py
--rw-r--r--   0        0        0     8705 2024-04-26 17:04:29.639337 langchain_google_genai-1.0.3/langchain_google_genai/_function_utils.py
--rw-r--r--   0        0        0    18736 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/_genai_extension.py
--rw-r--r--   0        0        0    29969 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/chat_models.py
--rw-r--r--   0        0        0     4807 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/embeddings.py
--rw-r--r--   0        0        0     4303 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/genai_aqa.py
--rw-r--r--   0        0        0    16139 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/google_vector_store.py
--rw-r--r--   0        0        0    13518 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/llms.py
--rw-r--r--   0        0        0        0 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/langchain_google_genai/py.typed
--rw-r--r--   0        0        0     3013 2024-04-26 17:04:29.643337 langchain_google_genai-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 langchain_google_genai-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2875 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/README.md
+-rw-r--r--   0        0        0     2758 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/__init__.py
+-rw-r--r--   0        0        0     1576 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_common.py
+-rw-r--r--   0        0        0      197 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_enums.py
+-rw-r--r--   0        0        0     8232 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_function_utils.py
+-rw-r--r--   0        0        0    20769 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_genai_extension.py
+-rw-r--r--   0        0        0     4999 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_image_utils.py
+-rw-r--r--   0        0        0    33014 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/chat_models.py
+-rw-r--r--   0        0        0     6578 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/embeddings.py
+-rw-r--r--   0        0        0     4303 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/genai_aqa.py
+-rw-r--r--   0        0        0    16139 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/google_vector_store.py
+-rw-r--r--   0        0        0    13431 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/llms.py
+-rw-r--r--   0        0        0        0 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/py.typed
+-rw-r--r--   0        0        0     3019 2024-05-16 13:42:50.390237 langchain_google_genai-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 langchain_google_genai-1.0.4/PKG-INFO
```

### Comparing `langchain_google_genai-1.0.3/LICENSE` & `langchain_google_genai-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.3/README.md` & `langchain_google_genai-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.3/langchain_google_genai/__init__.py` & `langchain_google_genai-1.0.4/langchain_google_genai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 llm = ChatGoogleGenerativeAI(model="gemini-pro")
 llm.invoke("Sing a ballad of LangChain.")
 ```
 
 ## Using LLMs
 
 The package also supports generating text with Google's models.
-    
+
 ```python
 from langchain_google_genai import GoogleGenerativeAI
 
 llm = GoogleGenerativeAI(model="gemini-pro")
 llm.invoke("Once upon a time, a library called LangChain")
 ```
```

### Comparing `langchain_google_genai-1.0.3/langchain_google_genai/_function_utils.py` & `langchain_google_genai-1.0.4/langchain_google_genai/_function_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from __future__ import annotations
 
 from typing import (
     Any,
+    Callable,
     Dict,
     List,
     Literal,
     Optional,
     Sequence,
     Type,
     TypedDict,
     Union,
+    cast,
 )
 
 import google.ai.generativelanguage as glm
-from google.generativeai.types import Tool as GoogleTool  # type: ignore[import]
-from google.generativeai.types.content_types import (  # type: ignore[import]
-    FunctionCallingConfigType,
-    FunctionDeclarationType,
-    ToolDict,
-    ToolType,
+from google.ai.generativelanguage import (
+    FunctionCallingConfig,
+    FunctionDeclaration,
+)
+from google.ai.generativelanguage import (
+    Tool as GoogleTool,
 )
 from langchain_core.pydantic_v1 import BaseModel
 from langchain_core.tools import BaseTool
 from langchain_core.tools import tool as callable_as_lc_tool
 from langchain_core.utils.json_schema import dereference_refs
 
 TYPE_ENUM = {
@@ -32,59 +34,49 @@
     "boolean": glm.Type.BOOLEAN,
     "array": glm.Type.ARRAY,
     "object": glm.Type.OBJECT,
 }
 
 TYPE_ENUM_REVERSE = {v: k for k, v in TYPE_ENUM.items()}
 
+_FunctionDeclarationLike = Union[
+    BaseTool, Type[BaseModel], dict, Callable, FunctionDeclaration
+]
+
+
+class _ToolDict(TypedDict):
+    function_declarations: Sequence[_FunctionDeclarationLike]
+
 
 def convert_to_genai_function_declarations(
     tool: Union[
-        GoogleTool, ToolDict, FunctionDeclarationType, Sequence[FunctionDeclarationType]
+        GoogleTool,
+        _ToolDict,
+        _FunctionDeclarationLike,
+        Sequence[_FunctionDeclarationLike],
     ],
-) -> ToolType:
-    """Convert any tool-like object to a ToolType.
-
-    https://github.com/google-gemini/generative-ai-python/blob/668695ebe3e9de496a36eeb95cb2ed2faba9b939/google/generativeai/types/content_types.py#L574
-    """
+) -> GoogleTool:
     if isinstance(tool, GoogleTool):
-        return tool
-    # check whether a dict is supported by glm, otherwise we parse it explicitly
-    if isinstance(tool, dict):
-        first_function_declaration = tool.get("function_declarations", [None])[0]
-        if isinstance(first_function_declaration, glm.FunctionDeclaration):
-            return tool
-        schema = None
-        try:
-            schema = first_function_declaration.parameters
-        except AttributeError:
-            pass
-        if schema is None:
-            schema = first_function_declaration.get("parameters")
-        if schema is None or isinstance(schema, glm.Schema):
-            return tool
-        return glm.Tool(
+        return cast(GoogleTool, tool)
+    if isinstance(tool, type) and issubclass(tool, BaseModel):
+        return GoogleTool(function_declarations=[_convert_to_genai_function(tool)])
+    if callable(tool):
+        return _convert_tool_to_genai_function(callable_as_lc_tool()(tool))
+    if isinstance(tool, list):
+        return convert_to_genai_function_declarations({"function_declarations": tool})
+    if isinstance(tool, dict) and "function_declarations" in tool:
+        return GoogleTool(
             function_declarations=[
                 _convert_to_genai_function(fc) for fc in tool["function_declarations"]
             ],
         )
-    elif isinstance(tool, type) and issubclass(tool, BaseModel):
-        return glm.Tool(function_declarations=[_convert_to_genai_function(tool)])
-    elif callable(tool):
-        return _convert_tool_to_genai_function(callable_as_lc_tool()(tool))
-    elif isinstance(tool, list):
-        return glm.Tool(
-            function_declarations=[_convert_to_genai_function(fc) for fc in tool]
-        )
-    return glm.Tool(function_declarations=[_convert_to_genai_function(tool)])
+    return GoogleTool(function_declarations=[_convert_to_genai_function(tool)])  # type: ignore[arg-type]
 
 
-def tool_to_dict(tool: Union[glm.Tool, GoogleTool]) -> ToolDict:
-    if isinstance(tool, GoogleTool):
-        tool = tool._proto
+def tool_to_dict(tool: GoogleTool) -> _ToolDict:
     function_declarations = []
     for function_declaration_proto in tool.function_declarations:
         properties: Dict[str, Any] = {}
         for property in function_declaration_proto.parameters.properties:
             property_type = function_declaration_proto.parameters.properties[
                 property
             ].type
@@ -104,46 +96,45 @@
             function_declaration["parameters"][  # type: ignore[index]
                 "required"
             ] = function_declaration_proto.parameters.required
         function_declarations.append(function_declaration)
     return {"function_declarations": function_declarations}
 
 
-def _convert_to_genai_function(fc: FunctionDeclarationType) -> glm.FunctionDeclaration:
+def _convert_to_genai_function(fc: _FunctionDeclarationLike) -> FunctionDeclaration:
     if isinstance(fc, BaseTool):
         return _convert_tool_to_genai_function(fc)
     elif isinstance(fc, type) and issubclass(fc, BaseModel):
         return _convert_pydantic_to_genai_function(fc)
     elif callable(fc):
         return _convert_tool_to_genai_function(callable_as_lc_tool()(fc))
     elif isinstance(fc, dict):
-        return glm.FunctionDeclaration(
-            name=fc["name"],
-            description=fc.get("description"),
-            parameters={
+        formatted_fc = {"name": fc["name"], "description": fc.get("description")}
+        if "parameters" in fc:
+            formatted_fc["parameters"] = {
                 "properties": {
                     k: {
                         "type_": TYPE_ENUM[v["type"]],
                         "description": v.get("description"),
                     }
                     for k, v in fc["parameters"]["properties"].items()
                 },
-                "required": fc["parameters"].get("required", []),
+                "required": fc.get("parameters", []).get("required", []),
                 "type_": TYPE_ENUM[fc["parameters"]["type"]],
-            },
-        )
+            }
+        return FunctionDeclaration(**formatted_fc)
     else:
         raise ValueError(f"Unsupported function call type {fc}")
 
 
-def _convert_tool_to_genai_function(tool: BaseTool) -> glm.FunctionDeclaration:
+def _convert_tool_to_genai_function(tool: BaseTool) -> FunctionDeclaration:
     if tool.args_schema:
         schema = dereference_refs(tool.args_schema.schema())
         schema.pop("definitions", None)
-        return glm.FunctionDeclaration(
+        return FunctionDeclaration(
             name=tool.name or schema["title"],
             description=tool.description or schema["description"],
             parameters={
                 "properties": {
                     k: {
                         "type_": TYPE_ENUM[v["type"]],
                         "description": v.get("description"),
@@ -151,33 +142,33 @@
                     for k, v in schema["properties"].items()
                 },
                 "required": schema.get("required", []),
                 "type_": TYPE_ENUM[schema["type"]],
             },
         )
     else:
-        return glm.FunctionDeclaration(
+        return FunctionDeclaration(
             name=tool.name,
             description=tool.description,
             parameters={
                 "properties": {
                     "__arg1": {"type_": TYPE_ENUM["string"]},
                 },
                 "required": ["__arg1"],
                 "type_": TYPE_ENUM["object"],
             },
         )
 
 
 def _convert_pydantic_to_genai_function(
     pydantic_model: Type[BaseModel],
-) -> glm.FunctionDeclaration:
+) -> FunctionDeclaration:
     schema = dereference_refs(pydantic_model.schema())
     schema.pop("definitions", None)
-    return glm.FunctionDeclaration(
+    return FunctionDeclaration(
         name=schema["title"],
         description=schema.get("description", ""),
         parameters={
             "properties": {
                 k: {
                     "type_": TYPE_ENUM[v["type"]],
                     "description": v.get("description"),
@@ -191,16 +182,21 @@
 
 
 _ToolChoiceType = Union[
     dict, List[str], str, Literal["auto", "none", "any"], Literal[True]
 ]
 
 
+class _FunctionCallingConfigDict(TypedDict):
+    mode: Union[FunctionCallingConfig.Mode, str]
+    allowed_function_names: Optional[List[str]]
+
+
 class _ToolConfigDict(TypedDict):
-    function_calling_config: FunctionCallingConfigType
+    function_calling_config: _FunctionCallingConfigDict
 
 
 def _tool_choice_to_tool_config(
     tool_choice: _ToolChoiceType,
     all_names: List[str],
 ) -> _ToolConfigDict:
     allowed_function_names: Optional[List[str]] = None
```

### Comparing `langchain_google_genai-1.0.3/langchain_google_genai/_genai_extension.py` & `langchain_google_genai-1.0.4/langchain_google_genai/_genai_extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 import logging
 import re
 from dataclasses import dataclass
 from typing import Any, Dict, Iterator, List, MutableSequence, Optional
 
 import google.ai.generativelanguage as genai
 import langchain_core
+from google.ai.generativelanguage_v1beta import (
+    GenerativeServiceAsyncClient as v1betaGenerativeServiceAsyncClient,
+)
+from google.ai.generativelanguage_v1beta import (
+    GenerativeServiceClient as v1betaGenerativeServiceClient,
+)
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as gapi_exception
 from google.api_core import gapic_v1
 from google.auth import credentials, exceptions  # type: ignore
 from google.protobuf import timestamp_pb2
 
 _logger = logging.getLogger(__name__)
@@ -221,23 +227,74 @@
         client_info=gapic_v1.client_info.ClientInfo(user_agent=_USER_AGENT),
         client_options=client_options_lib.ClientOptions(
             api_endpoint=_config.api_endpoint
         ),
     )
 
 
-def build_generative_service() -> genai.GenerativeServiceClient:
-    credentials = _get_credentials()
-    return genai.GenerativeServiceClient(
+def _prepare_config(
+    credentials: Optional[credentials.Credentials] = None,
+    api_key: Optional[str] = None,
+    client_options: Optional[Dict[str, Any]] = None,
+    client_info: Optional[gapic_v1.client_info.ClientInfo] = None,
+    transport: Optional[str] = None,
+) -> Dict[str, Any]:
+    formatted_client_options = {"api_endpoint": _config.api_endpoint}
+    if client_options:
+        formatted_client_options.update(**client_options)
+    if not credentials and api_key:
+        formatted_client_options["api_key"] = api_key
+    elif not credentials and not api_key:
+        credentials = _get_credentials()
+    client_info = (
+        client_info
+        if client_info
+        else gapic_v1.client_info.ClientInfo(user_agent=_USER_AGENT)
+    )
+    config = {
+        "credentials": credentials,
+        "client_info": client_info,
+        "client_options": client_options_lib.ClientOptions(**formatted_client_options),
+        "transport": transport,
+    }
+    return {k: v for k, v in config.items() if v is not None}
+
+
+def build_generative_service(
+    credentials: Optional[credentials.Credentials] = None,
+    api_key: Optional[str] = None,
+    client_options: Optional[Dict[str, Any]] = None,
+    client_info: Optional[gapic_v1.client_info.ClientInfo] = None,
+    transport: Optional[str] = None,
+) -> v1betaGenerativeServiceClient:
+    config = _prepare_config(
         credentials=credentials,
-        client_info=gapic_v1.client_info.ClientInfo(user_agent=_USER_AGENT),
-        client_options=client_options_lib.ClientOptions(
-            api_endpoint=_config.api_endpoint
-        ),
+        api_key=api_key,
+        client_options=client_options,
+        transport=transport,
+        client_info=client_info,
+    )
+    return v1betaGenerativeServiceClient(**config)
+
+
+def build_generative_async_service(
+    credentials: Optional[credentials.Credentials],
+    api_key: Optional[str] = None,
+    client_options: Optional[Dict[str, Any]] = None,
+    client_info: Optional[gapic_v1.client_info.ClientInfo] = None,
+    transport: Optional[str] = None,
+) -> v1betaGenerativeServiceAsyncClient:
+    config = _prepare_config(
+        credentials=credentials,
+        api_key=api_key,
+        client_options=client_options,
+        transport=transport,
+        client_info=client_info,
     )
+    return v1betaGenerativeServiceAsyncClient(**config)
 
 
 def list_corpora(
     *,
     client: genai.RetrieverServiceClient,
 ) -> Iterator[Corpus]:
     for corpus in client.list_corpora(
```

### Comparing `langchain_google_genai-1.0.3/langchain_google_genai/chat_models.py` & `langchain_google_genai-1.0.4/langchain_google_genai/chat_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,22 +19,31 @@
     Sequence,
     Tuple,
     Union,
     cast,
 )
 from urllib.parse import urlparse
 
-import google.ai.generativelanguage as glm
 import google.api_core
 
 # TODO: remove ignore once the google package is published with types
-import google.generativeai as genai  # type: ignore[import]
 import proto  # type: ignore[import]
 import requests
-from google.generativeai.types import SafetySettingDict  # type: ignore[import]
+from google.ai.generativelanguage_v1beta.types import (
+    Candidate,
+    Content,
+    FunctionCall,
+    FunctionResponse,
+    GenerateContentRequest,
+    GenerateContentResponse,
+    GenerationConfig,
+    Part,
+    SafetySetting,
+    ToolConfig,
+)
 from google.generativeai.types import Tool as GoogleTool  # type: ignore[import]
 from google.generativeai.types.content_types import (  # type: ignore[import]
     FunctionDeclarationType,
     ToolDict,
 )
 from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForLLMRun,
@@ -52,34 +61,41 @@
     SystemMessage,
     ToolCall,
     ToolCallChunk,
     ToolMessage,
 )
 from langchain_core.output_parsers.openai_tools import parse_tool_calls
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
-from langchain_core.pydantic_v1 import SecretStr, root_validator
+from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
 from langchain_core.runnables import Runnable
 from langchain_core.utils import get_from_dict_or_env
 from tenacity import (
     before_sleep_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
-from langchain_google_genai._common import GoogleGenerativeAIError
+from langchain_google_genai._common import (
+    GoogleGenerativeAIError,
+    SafetySettingDict,
+    get_client_info,
+)
 from langchain_google_genai._function_utils import (
     _tool_choice_to_tool_config,
     _ToolChoiceType,
     _ToolConfigDict,
     convert_to_genai_function_declarations,
     tool_to_dict,
 )
-from langchain_google_genai.llms import GoogleModelFamily, _BaseGoogleGenerativeAI
+from langchain_google_genai._image_utils import ImageBytesLoader
+from langchain_google_genai.llms import _BaseGoogleGenerativeAI
+
+from . import _genai_extension as genaix
 
 IMAGE_TYPES: Tuple = ()
 try:
     import PIL
     from PIL.Image import Image
 
     IMAGE_TYPES = IMAGE_TYPES + (Image,)
@@ -275,94 +291,98 @@
             )
     except Exception as e:
         raise ValueError(f"Unable to process the provided image source: {e}")
 
 
 def _convert_to_parts(
     raw_content: Union[str, Sequence[Union[str, dict]]],
-) -> List[genai.types.PartType]:
+) -> List[Part]:
     """Converts a list of LangChain messages into a google parts."""
     parts = []
     content = [raw_content] if isinstance(raw_content, str) else raw_content
+    image_loader = ImageBytesLoader()
     for part in content:
         if isinstance(part, str):
-            parts.append(genai.types.PartDict(text=part))
+            parts.append(Part(text=part))
         elif isinstance(part, Mapping):
             # OpenAI Format
             if _is_openai_parts_format(part):
                 if part["type"] == "text":
-                    parts.append({"text": part["text"]})
+                    parts.append(Part(text=part["text"]))
                 elif part["type"] == "image_url":
                     img_url = part["image_url"]
                     if isinstance(img_url, dict):
                         if "url" not in img_url:
                             raise ValueError(
                                 f"Unrecognized message image format: {img_url}"
                             )
                         img_url = img_url["url"]
-                    parts.append({"inline_data": _url_to_pil(img_url)})
+                    parts.append(image_loader.load_part(img_url))
                 else:
                     raise ValueError(f"Unrecognized message part type: {part['type']}")
             else:
                 # Yolo
                 logger.warning(
                     "Unrecognized message part format. Assuming it's a text part."
                 )
-                parts.append(part)
+                parts.append(Part(text=str(part)))
         else:
             # TODO: Maybe some of Google's native stuff
             # would hit this branch.
             raise ChatGoogleGenerativeAIError(
                 "Gemini only supports text and inline_data parts."
             )
     return parts
 
 
 def _parse_chat_history(
     input_messages: Sequence[BaseMessage], convert_system_message_to_human: bool = False
-) -> Tuple[Optional[genai.types.ContentDict], List[genai.types.ContentDict]]:
-    messages: List[genai.types.MessageDict] = []
+) -> Tuple[Optional[Content], List[Content]]:
+    messages: List[Content] = []
 
     if convert_system_message_to_human:
         warnings.warn("Convert_system_message_to_human will be deprecated!")
 
-    system_instruction: Optional[genai.types.ContentDict] = None
+    system_instruction: Optional[Content] = None
     for i, message in enumerate(input_messages):
         if i == 0 and isinstance(message, SystemMessage):
-            system_instruction = _convert_to_parts(message.content)
+            system_instruction = Content(parts=_convert_to_parts(message.content))
             continue
         elif isinstance(message, AIMessage):
             role = "model"
             raw_function_call = message.additional_kwargs.get("function_call")
             if raw_function_call:
-                function_call = glm.FunctionCall(
+                function_call = FunctionCall(
                     {
                         "name": raw_function_call["name"],
                         "args": json.loads(raw_function_call["arguments"]),
                     }
                 )
-                parts = [glm.Part(function_call=function_call)]
+                parts = [Part(function_call=function_call)]
             else:
                 parts = _convert_to_parts(message.content)
         elif isinstance(message, HumanMessage):
             role = "user"
             parts = _convert_to_parts(message.content)
+            if i == 1 and convert_system_message_to_human and system_instruction:
+                parts = [p for p in system_instruction.parts] + parts
+                system_instruction = None
         elif isinstance(message, FunctionMessage):
             role = "user"
             response: Any
             if not isinstance(message.content, str):
                 response = message.content
             else:
                 try:
                     response = json.loads(message.content)
                 except json.JSONDecodeError:
                     response = message.content  # leave as str representation
             parts = [
-                glm.Part(
-                    function_response=glm.FunctionResponse(
+                Part(
+                    function_response=FunctionResponse(
                         name=message.name,
                         response=(
                             {"output": response}
                             if not isinstance(response, dict)
                             else response
                         ),
                     )
@@ -387,36 +407,36 @@
                 tool_response = message.content
             else:
                 try:
                     tool_response = json.loads(message.content)
                 except json.JSONDecodeError:
                     tool_response = message.content  # leave as str representation
             parts = [
-                glm.Part(
-                    function_response=glm.FunctionResponse(
+                Part(
+                    function_response=FunctionResponse(
                         name=name,
                         response=(
                             {"output": tool_response}
                             if not isinstance(tool_response, dict)
                             else tool_response
                         ),
                     )
                 )
             ]
         else:
             raise ValueError(
                 f"Unexpected message with type {type(message)} at the position {i}."
             )
 
-        messages.append({"role": role, "parts": parts})
+        messages.append(Content(role=role, parts=parts))
     return system_instruction, messages
 
 
 def _parse_response_candidate(
-    response_candidate: glm.Candidate, streaming: bool = False
+    response_candidate: Candidate, streaming: bool = False
 ) -> AIMessage:
     content: Union[None, str, List[str]] = None
     additional_kwargs = {}
     tool_calls = []
     invalid_tool_calls = []
     tool_call_chunks = []
 
@@ -495,15 +515,15 @@
         additional_kwargs=additional_kwargs,
         tool_calls=tool_calls,
         invalid_tool_calls=invalid_tool_calls,
     )
 
 
 def _response_to_result(
-    response: glm.GenerateContentResponse,
+    response: GenerateContentResponse,
     stream: bool = False,
 ) -> ChatResult:
     """Converts a PaLM API response into a LangChain ChatResult."""
     llm_output = {"prompt_feedback": proto.Message.to_dict(response.prompt_feedback)}
 
     generations: List[ChatGeneration] = []
 
@@ -553,14 +573,18 @@
             from langchain_google_genai import ChatGoogleGenerativeAI
             chat = ChatGoogleGenerativeAI(model="gemini-pro")
             chat.invoke("Write me a ballad about LangChain")
 
     """
 
     client: Any  #: :meta private:
+    async_client: Any  #: :meta private:
+    default_metadata: Sequence[Tuple[str, str]] = Field(
+        default_factory=list
+    )  #: :meta private:
 
     convert_system_message_to_human: bool = False
     """Whether to merge any leading SystemMessage into the following HumanMessage.
     
     Gemini does not support system messages; any unsupported messages will 
     raise an error."""
 
@@ -578,230 +602,284 @@
     @classmethod
     def is_lc_serializable(self) -> bool:
         return True
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validates params and passes them to google-generativeai package."""
-        additional_headers = values.get("additional_headers") or {}
-        default_metadata = tuple(additional_headers.items())
-
-        if values.get("credentials"):
-            genai.configure(
-                credentials=values.get("credentials"),
-                transport=values.get("transport"),
-                client_options=values.get("client_options"),
-                default_metadata=default_metadata,
-            )
-        else:
-            google_api_key = get_from_dict_or_env(
-                values, "google_api_key", "GOOGLE_API_KEY"
-            )
-            if isinstance(google_api_key, SecretStr):
-                google_api_key = google_api_key.get_secret_value()
-
-            genai.configure(
-                api_key=google_api_key,
-                transport=values.get("transport"),
-                client_options=values.get("client_options"),
-                default_metadata=default_metadata,
-            )
         if (
             values.get("temperature") is not None
             and not 0 <= values["temperature"] <= 1
         ):
             raise ValueError("temperature must be in the range [0.0, 1.0]")
 
         if values.get("top_p") is not None and not 0 <= values["top_p"] <= 1:
             raise ValueError("top_p must be in the range [0.0, 1.0]")
 
         if values.get("top_k") is not None and values["top_k"] <= 0:
             raise ValueError("top_k must be positive")
-        model = values["model"]
-        values["client"] = genai.GenerativeModel(model_name=model)
+
+        if not values["model"].startswith("models/"):
+            values["model"] = f"models/{values['model']}"
+
+        additional_headers = values.get("additional_headers") or {}
+        values["default_metadata"] = tuple(additional_headers.items())
+        client_info = get_client_info("ChatGoogleGenerativeAI")
+        google_api_key = None
+        if not values.get("credentials"):
+            google_api_key = get_from_dict_or_env(
+                values, "google_api_key", "GOOGLE_API_KEY"
+            )
+            if isinstance(google_api_key, SecretStr):
+                google_api_key = google_api_key.get_secret_value()
+        transport: Optional[str] = values.get("transport")
+        values["client"] = genaix.build_generative_service(
+            credentials=values.get("credentials"),
+            api_key=google_api_key,
+            client_info=client_info,
+            client_options=values.get("client_options"),
+            transport=transport,
+        )
+        values["async_client"] = genaix.build_generative_async_service(
+            credentials=values.get("credentials"),
+            api_key=google_api_key,
+            client_info=client_info,
+            client_options=values.get("client_options"),
+            transport=transport,
+        )
+
         return values
 
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Get the identifying parameters."""
         return {
             "model": self.model,
             "temperature": self.temperature,
             "top_k": self.top_k,
             "n": self.n,
             "safety_settings": self.safety_settings,
         }
 
     def _prepare_params(
-        self, stop: Optional[List[str]], **kwargs: Any
-    ) -> Dict[str, Any]:
+        self,
+        stop: Optional[List[str]],
+        generation_config: Optional[Dict[str, Any]] = None,
+    ) -> GenerationConfig:
         gen_config = {
             k: v
             for k, v in {
                 "candidate_count": self.n,
                 "temperature": self.temperature,
                 "stop_sequences": stop,
                 "max_output_tokens": self.max_output_tokens,
                 "top_k": self.top_k,
                 "top_p": self.top_p,
             }.items()
             if v is not None
         }
-        if "generation_config" in kwargs:
-            gen_config = {**gen_config, **kwargs.pop("generation_config")}
-        params = {"generation_config": gen_config, **kwargs}
-        return params
+        if generation_config:
+            gen_config = {**gen_config, **generation_config}
+        return GenerationConfig(**gen_config)
 
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
+        *,
+        tools: Optional[Sequence[Union[ToolDict, GoogleTool]]] = None,
+        functions: Optional[Sequence[FunctionDeclarationType]] = None,
+        safety_settings: Optional[SafetySettingDict] = None,
+        tool_config: Optional[Union[Dict, _ToolConfigDict]] = None,
+        generation_config: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> ChatResult:
-        params, chat, message = self._prepare_chat(
+        request = self._prepare_request(
             messages,
             stop=stop,
-            **kwargs,
+            tools=tools,
+            functions=functions,
+            safety_settings=safety_settings,
+            tool_config=tool_config,
+            generation_config=generation_config,
         )
-        response: genai.types.GenerateContentResponse = _chat_with_retry(
-            content=message,
-            **params,
-            generation_method=chat.send_message,
+        response: GenerateContentResponse = _chat_with_retry(
+            request=request,
+            **kwargs,
+            generation_method=self.client.generate_content,
+            metadata=self.default_metadata,
         )
         return _response_to_result(response)
 
     async def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
+        *,
+        tools: Optional[Sequence[Union[ToolDict, GoogleTool]]] = None,
+        functions: Optional[Sequence[FunctionDeclarationType]] = None,
+        safety_settings: Optional[SafetySettingDict] = None,
+        tool_config: Optional[Union[Dict, _ToolConfigDict]] = None,
+        generation_config: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> ChatResult:
-        params, chat, message = self._prepare_chat(
+        request = self._prepare_request(
             messages,
             stop=stop,
-            **kwargs,
+            tools=tools,
+            functions=functions,
+            safety_settings=safety_settings,
+            tool_config=tool_config,
+            generation_config=generation_config,
         )
-        response: genai.types.GenerateContentResponse = await _achat_with_retry(
-            content=message,
-            **params,
-            generation_method=chat.send_message_async,
+        response: GenerateContentResponse = await _achat_with_retry(
+            request=request,
+            **kwargs,
+            generation_method=self.async_client.generate_content,
+            metadata=self.default_metadata,
         )
         return _response_to_result(response)
 
     def _stream(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
+        *,
+        tools: Optional[Sequence[Union[ToolDict, GoogleTool]]] = None,
+        functions: Optional[Sequence[FunctionDeclarationType]] = None,
+        safety_settings: Optional[SafetySettingDict] = None,
+        tool_config: Optional[Union[Dict, _ToolConfigDict]] = None,
+        generation_config: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
-        params, chat, message = self._prepare_chat(
+        request = self._prepare_request(
             messages,
             stop=stop,
+            tools=tools,
+            functions=functions,
+            safety_settings=safety_settings,
+            tool_config=tool_config,
+            generation_config=generation_config,
+        )
+        response: GenerateContentResponse = _chat_with_retry(
+            request=request,
+            generation_method=self.client.stream_generate_content,
             **kwargs,
-        )
-        response: genai.types.GenerateContentResponse = _chat_with_retry(
-            content=message,
-            **params,
-            generation_method=chat.send_message,
-            stream=True,
+            metadata=self.default_metadata,
         )
         for chunk in response:
             _chat_result = _response_to_result(chunk, stream=True)
             gen = cast(ChatGenerationChunk, _chat_result.generations[0])
 
             if run_manager:
                 run_manager.on_llm_new_token(gen.text)
             yield gen
 
     async def _astream(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
+        *,
+        tools: Optional[Sequence[Union[ToolDict, GoogleTool]]] = None,
+        functions: Optional[Sequence[FunctionDeclarationType]] = None,
+        safety_settings: Optional[SafetySettingDict] = None,
+        tool_config: Optional[Union[Dict, _ToolConfigDict]] = None,
+        generation_config: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> AsyncIterator[ChatGenerationChunk]:
-        params, chat, message = self._prepare_chat(
+        request = self._prepare_request(
             messages,
             stop=stop,
-            **kwargs,
+            tools=tools,
+            functions=functions,
+            safety_settings=safety_settings,
+            tool_config=tool_config,
+            generation_config=generation_config,
         )
         async for chunk in await _achat_with_retry(
-            content=message,
-            **params,
-            generation_method=chat.send_message_async,
-            stream=True,
+            request=request,
+            generation_method=self.async_client.stream_generate_content,
+            **kwargs,
+            metadata=self.default_metadata,
         ):
             _chat_result = _response_to_result(chunk, stream=True)
             gen = cast(ChatGenerationChunk, _chat_result.generations[0])
 
             if run_manager:
                 await run_manager.on_llm_new_token(gen.text)
             yield gen
 
-    def _prepare_chat(
+    def _prepare_request(
         self,
         messages: List[BaseMessage],
+        *,
         stop: Optional[List[str]] = None,
         tools: Optional[Sequence[Union[ToolDict, GoogleTool]]] = None,
         functions: Optional[Sequence[FunctionDeclarationType]] = None,
         safety_settings: Optional[SafetySettingDict] = None,
         tool_config: Optional[Union[Dict, _ToolConfigDict]] = None,
-        **kwargs: Any,
-    ) -> Tuple[Dict[str, Any], genai.ChatSession, genai.types.ContentDict]:
-        client = self.client
+        generation_config: Optional[Dict[str, Any]] = None,
+    ) -> Tuple[GenerateContentRequest, Dict[str, Any]]:
         formatted_tools = None
         if tools:
             formatted_tools = [
                 convert_to_genai_function_declarations(tool) for tool in tools
             ]
         elif functions:
             formatted_tools = [convert_to_genai_function_declarations(functions)]
 
-        if formatted_tools or safety_settings:
-            client = genai.GenerativeModel(
-                model_name=self.model,
-                tools=formatted_tools,
-                safety_settings=safety_settings,
-            )
-
-        params = self._prepare_params(stop, tool_config=tool_config, **kwargs)
         system_instruction, history = _parse_chat_history(
             messages,
             convert_system_message_to_human=self.convert_system_message_to_human,
         )
-        message = history.pop()
-        if self.client._system_instruction != system_instruction:
-            self.client = genai.GenerativeModel(
-                model_name=self.model, system_instruction=system_instruction
-            )
-        chat = client.start_chat(history=history)
-        return params, chat, message
+        formatted_tool_config = None
+        if tool_config:
+            formatted_tool_config = ToolConfig(
+                function_calling_config=tool_config["function_calling_config"]
+            )
+        formatted_safety_settings = []
+        if safety_settings:
+            formatted_safety_settings = [
+                SafetySetting(category=c, threshold=t)
+                for c, t in safety_settings.items()
+            ]
+        request = GenerateContentRequest(
+            model=self.model,
+            contents=history,
+            tools=formatted_tools,
+            tool_config=formatted_tool_config,
+            safety_settings=formatted_safety_settings,
+            generation_config=self._prepare_params(
+                stop, generation_config=generation_config
+            ),
+        )
+        if system_instruction:
+            request.system_instruction = system_instruction
+
+        return request
 
     def get_num_tokens(self, text: str) -> int:
         """Get the number of tokens present in the text.
 
         Useful for checking if an input will fit in a model's context window.
 
         Args:
             text: The string input to tokenize.
 
         Returns:
             The integer number of tokens in the text.
         """
-        if self._model_family == GoogleModelFamily.GEMINI:
-            result = self.client.count_tokens(text)
-            token_count = result.total_tokens
-        else:
-            result = self.client.count_text_tokens(model=self.model, prompt=text)
-            token_count = result["token_count"]
-
-        return token_count
+        result = self.client.count_tokens(
+            model=self.model, contents=[Content(parts=[Part(text=text)])]
+        )
+        return result.total_tokens
 
     def bind_tools(
         self,
         tools: Sequence[Union[ToolDict, GoogleTool]],
         tool_config: Optional[Union[Dict, _ToolConfigDict]] = None,
         *,
         tool_choice: Optional[Union[_ToolChoiceType, bool]] = None,
@@ -824,11 +902,13 @@
                 "Must specify at most one of tool_choice and tool_config, received "
                 f"both:\n\n{tool_choice=}\n\n{tool_config=}"
             )
         # Bind dicts for easier serialization/deserialization.
         genai_tools = [tool_to_dict(convert_to_genai_function_declarations(tools))]
         if tool_choice:
             all_names = [
-                f["name"] for t in genai_tools for f in t["function_declarations"]
+                f["name"]  # type: ignore[index]
+                for t in genai_tools
+                for f in t["function_declarations"]
             ]
             tool_config = _tool_choice_to_tool_config(tool_choice, all_names)
         return self.bind(tools=genai_tools, tool_config=tool_config, **kwargs)
```

### Comparing `langchain_google_genai-1.0.3/langchain_google_genai/embeddings.py` & `langchain_google_genai-1.0.4/langchain_google_genai/embeddings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from typing import Any, Dict, List, Optional
 
 # TODO: remove ignore once the google package is published with types
-import google.generativeai as genai  # type: ignore[import]
+from google.ai.generativelanguage_v1beta.types import (
+    BatchEmbedContentsRequest,
+    EmbedContentRequest,
+)
 from langchain_core.embeddings import Embeddings
 from langchain_core.pydantic_v1 import BaseModel, Field, SecretStr, root_validator
 from langchain_core.utils import get_from_dict_or_env
 
-from langchain_google_genai._common import GoogleGenerativeAIError
+from langchain_google_genai._common import (
+    GoogleGenerativeAIError,
+    get_client_info,
+)
+from langchain_google_genai._genai_extension import build_generative_service
 
 
 class GoogleGenerativeAIEmbeddings(BaseModel, Embeddings):
     """`Google Generative AI Embeddings`.
 
     To use, you must have either:
 
@@ -23,14 +30,15 @@
 
             from langchain_google_genai import GoogleGenerativeAIEmbeddings
 
             embeddings = GoogleGenerativeAIEmbeddings(model="models/embedding-001")
             embeddings.embed_query("What's our Q1 revenue?")
     """
 
+    client: Any  #: :meta private:
     model: str = Field(
         ...,
         description="The name of the embedding model to use. "
         "Example: models/embedding-001",
     )
     task_type: Optional[str] = Field(
         None,
@@ -66,70 +74,106 @@
         description="A dictionary of request options to pass to the Google API client."
         "Example: `{'timeout': 10}`",
     )
 
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validates params and passes them to google-generativeai package."""
-        if values.get("credentials"):
-            genai.configure(
-                credentials=values.get("credentials"),
-                transport=values.get("transport"),
-                client_options=values.get("client_options"),
-            )
-        else:
-            google_api_key = get_from_dict_or_env(
-                values, "google_api_key", "GOOGLE_API_KEY"
-            )
-            if isinstance(google_api_key, SecretStr):
-                google_api_key = google_api_key.get_secret_value()
-
-            genai.configure(
-                api_key=google_api_key,
-                transport=values.get("transport"),
-                client_options=values.get("client_options"),
-            )
+        google_api_key = get_from_dict_or_env(
+            values, "google_api_key", "GOOGLE_API_KEY"
+        )
+        client_info = get_client_info("GoogleGenerativeAIEmbeddings")
+
+        values["client"] = build_generative_service(
+            credentials=values.get("credentials"),
+            api_key=google_api_key,
+            client_info=client_info,
+            client_options=values.get("client_options"),
+        )
         return values
 
-    def _embed(
-        self, texts: List[str], task_type: str, title: Optional[str] = None
-    ) -> List[List[float]]:
-        task_type = self.task_type or "retrieval_document"
-        try:
-            result = genai.embed_content(
-                model=self.model,
-                content=texts,
-                task_type=task_type,
-                title=title,
-                request_options=self.request_options,
-            )
-        except Exception as e:
-            raise GoogleGenerativeAIError(f"Error embedding content: {e}") from e
-        return result["embedding"]
+    def _prepare_request(
+        self,
+        text: str,
+        task_type: Optional[str] = None,
+        title: Optional[str] = None,
+        output_dimensionality: Optional[int] = None,
+    ) -> EmbedContentRequest:
+        task_type = self.task_type or task_type or "RETRIEVAL_DOCUMENT"
+        # https://ai.google.dev/api/rest/v1/models/batchEmbedContents#EmbedContentRequest
+        request = EmbedContentRequest(
+            content={"parts": [{"text": text}]},
+            model=self.model,
+            task_type=task_type.upper(),
+            title=title,
+            output_dimensionality=output_dimensionality,
+        )
+        return request
 
     def embed_documents(
-        self, texts: List[str], batch_size: int = 5
+        self,
+        texts: List[str],
+        task_type: Optional[str] = None,
+        titles: Optional[List[str]] = None,
+        output_dimensionality: Optional[int] = None,
     ) -> List[List[float]]:
         """Embed a list of strings. Vertex AI currently
         sets a max batch size of 5 strings.
 
         Args:
             texts: List[str] The list of strings to embed.
             batch_size: [int] The batch size of embeddings to send to the model
+            task_type: task_type (https://ai.google.dev/api/rest/v1/TaskType)
+            titles: An optional list of titles for texts provided.
+            Only applicable when TaskType is RETRIEVAL_DOCUMENT.
+            output_dimensionality: Optional reduced dimension for the output embedding.
+            https://ai.google.dev/api/rest/v1/models/batchEmbedContents#EmbedContentRequest
 
         Returns:
             List of embeddings, one for each text.
         """
-        task_type = self.task_type or "retrieval_document"
-        return self._embed(texts, task_type=task_type)
+        titles = titles if titles else [None] * len(texts)  # type: ignore[list-item]
+        requests = [
+            self._prepare_request(
+                text=text,
+                task_type=task_type,
+                title=title,
+                output_dimensionality=output_dimensionality,
+            )
+            for text, title in zip(texts, titles)
+        ]
+
+        try:
+            result = self.client.batch_embed_contents(
+                BatchEmbedContentsRequest(requests=requests, model=self.model)
+            )
+        except Exception as e:
+            raise GoogleGenerativeAIError(f"Error embedding content: {e}") from e
+        return [e.values for e in result.embeddings]
 
-    def embed_query(self, text: str) -> List[float]:
+    def embed_query(
+        self,
+        text: str,
+        task_type: Optional[str] = None,
+        title: Optional[str] = None,
+        output_dimensionality: Optional[int] = None,
+    ) -> List[float]:
         """Embed a text.
 
         Args:
             text: The text to embed.
+            task_type: task_type (https://ai.google.dev/api/rest/v1/TaskType)
+            title: An optional title for the text.
+            Only applicable when TaskType is RETRIEVAL_DOCUMENT.
+            output_dimensionality: Optional reduced dimension for the output embedding.
+            https://ai.google.dev/api/rest/v1/models/batchEmbedContents#EmbedContentRequest
 
         Returns:
             Embedding for the text.
         """
-        task_type = self.task_type or "retrieval_query"
-        return self._embed([text], task_type=task_type)[0]
+        task_type = self.task_type or "RETRIEVAL_QUERY"
+        return self.embed_documents(
+            [text],
+            task_type=task_type,
+            titles=[title] if title else None,
+            output_dimensionality=output_dimensionality,
+        )[0]
```

### Comparing `langchain_google_genai-1.0.3/langchain_google_genai/genai_aqa.py` & `langchain_google_genai-1.0.4/langchain_google_genai/genai_aqa.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.3/langchain_google_genai/google_vector_store.py` & `langchain_google_genai-1.0.4/langchain_google_genai/google_vector_store.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.3/langchain_google_genai/llms.py` & `langchain_google_genai-1.0.4/langchain_google_genai/llms.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,14 @@
     """The default safety settings to use for all generations. 
     
         For example: 
 
             from google.generativeai.types.safety_types import HarmBlockThreshold, HarmCategory
 
             safety_settings = {
-                HarmCategory.HARM_CATEGORY_UNSPECIFIED: HarmBlockThreshold.BLOCK_NONE,
                 HarmCategory.HARM_CATEGORY_DANGEROUS_CONTENT: HarmBlockThreshold.BLOCK_MEDIUM_AND_ABOVE,
                 HarmCategory.HARM_CATEGORY_HATE_SPEECH: HarmBlockThreshold.BLOCK_ONLY_HIGH,
                 HarmCategory.HARM_CATEGORY_HARASSMENT: HarmBlockThreshold.BLOCK_LOW_AND_ABOVE,
                 HarmCategory.HARM_CATEGORY_SEXUALLY_EXPLICIT: HarmBlockThreshold.BLOCK_NONE,
             }
             """  # noqa: E501
```

### Comparing `langchain_google_genai-1.0.3/pyproject.toml` & `langchain_google_genai-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-google-genai"
-version = "1.0.3"
+version = "1.0.4"
 description = "An integration package connecting Google's genai package and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-google"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-google/tree/main/libs/genai"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-langchain-core = ">=0.1.45,<0.2"
+langchain-core = ">=0.1.45,<0.3"
 google-generativeai = "^0.5.2"
 pillow = { version = "^10.1.0", optional = true }
 
 [tool.poetry.extras]
 images = ["pillow"]
 
 [tool.poetry.group.test]
@@ -26,15 +26,15 @@
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 numpy = "^1.26.2"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
@@ -53,25 +53,25 @@
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
 types-requests = "^2.28.11.5"
 types-google-cloud-ndb = "^2.2.0.1"
 types-pillow = "^10.1.0.2"
 types-protobuf = "^4.24.0.20240302"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pillow = "^10.1.0"
 types-requests = "^2.31.0.10"
 types-pillow = "^10.1.0.2"
 types-google-cloud-ndb = "^2.2.0.1"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.ruff]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
```

### Comparing `langchain_google_genai-1.0.3/PKG-INFO` & `langchain_google_genai-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-google-genai
-Version: 1.0.3
+Version: 1.0.4
 Summary: An integration package connecting Google's genai package and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: images
 Requires-Dist: google-generativeai (>=0.5.2,<0.6.0)
-Requires-Dist: langchain-core (>=0.1.45,<0.2)
+Requires-Dist: langchain-core (>=0.1.45,<0.3)
 Requires-Dist: pillow (>=10.1.0,<11.0.0) ; extra == "images"
 Project-URL: Repository, https://github.com/langchain-ai/langchain-google
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-google/tree/main/libs/genai
 Description-Content-Type: text/markdown
 
 # langchain-google-genai
```

