# Comparing `tmp/groq-0.5.0.tar.gz` & `tmp/groq-0.6.0.tar.gz`

## Comparing `groq-0.5.0.tar` & `groq-0.6.0.tar`

### file list

```diff
@@ -1,50 +1,55 @@
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/__init__.py
--rw-r--r--   0        0        0    62500 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_base_client.py
--rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_compat.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_constants.py
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_files.py
--rw-r--r--   0        0        0    16432 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_qs.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_resource.py
--rw-r--r--   0        0        0    27935 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_response.py
--rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_streaming.py
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_types.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/py.typed
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_sync.py
--rw-r--r--   0        0        0    12805 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/lib/.keep
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/lib/chat_completion_chunk.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/__init__.py
--rw-r--r--   0        0        0     9494 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/models.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/audio/__init__.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/audio/audio.py
--rw-r--r--   0        0        0    10893 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/audio/transcriptions.py
--rw-r--r--   0        0        0     8857 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/audio/translations.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/chat/__init__.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/chat/chat.py
--rw-r--r--   0        0        0    18464 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/resources/chat/completions.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/model.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/model_list.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/translation.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/audio/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/audio/transcription.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/audio/transcription_create_params.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/audio/translation_create_params.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/chat/__init__.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/chat/chat_completion.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 groq-0.5.0/src/groq/types/chat/completion_create_params.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 groq-0.5.0/.gitignore
--rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 groq-0.5.0/LICENSE
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 groq-0.5.0/README.md
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 groq-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    12180 2020-02-02 00:00:00.000000 groq-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/__init__.py
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_base_client.py
+-rw-r--r--   0        0        0    16214 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_constants.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_qs.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_resource.py
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_response.py
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_streaming.py
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_types.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/lib/.keep
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/lib/chat_completion_chunk.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/__init__.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/embeddings.py
+-rw-r--r--   0        0        0     9563 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/models.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/audio/__init__.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/audio/audio.py
+-rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/audio/transcriptions.py
+-rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/audio/translations.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/chat/chat.py
+-rw-r--r--   0        0        0    18538 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/resources/chat/completions.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/create_embedding_response.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/embedding.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/embedding_create_params.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/model.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/model_list.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/__init__.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/transcription.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/transcription_create_params.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/transcription_create_response.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/translation.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/translation_create_params.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/audio/translation_create_response.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/chat/__init__.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 groq-0.6.0/src/groq/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 groq-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11334 2020-02-02 00:00:00.000000 groq-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 groq-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    13265 2020-02-02 00:00:00.000000 groq-0.6.0/PKG-INFO
```

### Comparing `groq-0.5.0/src/groq/__init__.py` & `groq-0.6.0/src/groq/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from . import types
-from ._types import NoneType, Transport, ProxiesTypes
+from ._types import NOT_GIVEN, NoneType, NotGiven, Transport, ProxiesTypes
 from ._utils import file_from_path
 from ._client import Groq, Client, Stream, Timeout, AsyncGroq, Transport, AsyncClient, AsyncStream, RequestOptions
 from ._models import BaseModel
 from ._version import __title__, __version__
 from ._response import APIResponse as APIResponse, AsyncAPIResponse as AsyncAPIResponse
+from ._constants import DEFAULT_TIMEOUT, DEFAULT_MAX_RETRIES, DEFAULT_CONNECTION_LIMITS
 from ._exceptions import (
     APIError,
     GroqError,
     ConflictError,
     NotFoundError,
     APIStatusError,
     RateLimitError,
@@ -19,23 +20,26 @@
     APIConnectionError,
     AuthenticationError,
     InternalServerError,
     PermissionDeniedError,
     UnprocessableEntityError,
     APIResponseValidationError,
 )
+from ._base_client import DefaultHttpxClient, DefaultAsyncHttpxClient
 from ._utils._logs import setup_logging as _setup_logging
 
 __all__ = [
     "types",
     "__version__",
     "__title__",
     "NoneType",
     "Transport",
     "ProxiesTypes",
+    "NotGiven",
+    "NOT_GIVEN",
     "GroqError",
     "APIError",
     "APIStatusError",
     "APITimeoutError",
     "APIConnectionError",
     "APIResponseValidationError",
     "BadRequestError",
@@ -52,14 +56,19 @@
     "AsyncClient",
     "Stream",
     "AsyncStream",
     "Groq",
     "AsyncGroq",
     "file_from_path",
     "BaseModel",
+    "DEFAULT_TIMEOUT",
+    "DEFAULT_MAX_RETRIES",
+    "DEFAULT_CONNECTION_LIMITS",
+    "DefaultHttpxClient",
+    "DefaultAsyncHttpxClient",
 ]
 
 _setup_logging()
 
 # Update the __module__ attribute for exported symbols so that
 # error messages point to this module instead of the module
 # it was originally defined in, e.g.
```

### Comparing `groq-0.5.0/src/groq/_base_client.py` & `groq-0.6.0/src/groq/_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     Iterator,
     Optional,
     Generator,
     AsyncIterator,
     cast,
     overload,
 )
-from functools import lru_cache
 from typing_extensions import Literal, override, get_origin
 
 import anyio
 import httpx
 import distro
 import pydantic
 from httpx import URL, Limits
@@ -57,31 +56,31 @@
     ProxiesTypes,
     RequestFiles,
     HttpxSendArgs,
     AsyncTransport,
     RequestOptions,
     ModelBuilderProtocol,
 )
-from ._utils import is_dict, is_list, is_given, is_mapping
+from ._utils import is_dict, is_list, is_given, lru_cache, is_mapping
 from ._compat import model_copy, model_dump
 from ._models import GenericModel, FinalRequestOptions, validate_type, construct_type
 from ._response import (
     APIResponse,
     BaseAPIResponse,
     AsyncAPIResponse,
     extract_response_type,
 )
 from ._constants import (
-    DEFAULT_LIMITS,
     DEFAULT_TIMEOUT,
     MAX_RETRY_DELAY,
     DEFAULT_MAX_RETRIES,
     INITIAL_RETRY_DELAY,
     RAW_RESPONSE_HEADER,
     OVERRIDE_CAST_TO_HEADER,
+    DEFAULT_CONNECTION_LIMITS,
 )
 from ._streaming import Stream, SSEDecoder, AsyncStream, SSEBytesDecoder
 from ._exceptions import (
     APIStatusError,
     APITimeoutError,
     APIConnectionError,
     APIResponseValidationError,
@@ -356,14 +355,19 @@
         self._proxies = proxies
         self._transport = transport
         self._custom_headers = custom_headers or {}
         self._custom_query = custom_query or {}
         self._strict_response_validation = _strict_response_validation
         self._idempotency_header = None
 
+        if max_retries is None:  # pyright: ignore[reportUnnecessaryComparison]
+            raise TypeError(
+                "max_retries cannot be None. If you want to disable retries, pass `0`; if you want unlimited retries, pass `math.inf` or a very high number; if you want the default behavior, pass `groq.DEFAULT_MAX_RETRIES`"
+            )
+
     def _enforce_trailing_slash(self, url: URL) -> URL:
         if url.raw_path.endswith(b"/"):
             return url
         return url.copy_with(raw_path=url.raw_path + b"/")
 
     def _make_status_error_from_response(
         self,
@@ -706,15 +710,35 @@
         log.debug("Not retrying")
         return False
 
     def _idempotency_key(self) -> str:
         return f"stainless-python-retry-{uuid.uuid4()}"
 
 
-class SyncHttpxClientWrapper(httpx.Client):
+class _DefaultHttpxClient(httpx.Client):
+    def __init__(self, **kwargs: Any) -> None:
+        kwargs.setdefault("timeout", DEFAULT_TIMEOUT)
+        kwargs.setdefault("limits", DEFAULT_CONNECTION_LIMITS)
+        kwargs.setdefault("follow_redirects", True)
+        super().__init__(**kwargs)
+
+
+if TYPE_CHECKING:
+    DefaultHttpxClient = httpx.Client
+    """An alias to `httpx.Client` that provides the same defaults that this SDK
+    uses internally.
+
+    This is useful because overriding the `http_client` with your own instance of
+    `httpx.Client` will result in httpx's defaults being used, not ours.
+    """
+else:
+    DefaultHttpxClient = _DefaultHttpxClient
+
+
+class SyncHttpxClientWrapper(DefaultHttpxClient):
     def __del__(self) -> None:
         try:
             self.close()
         except Exception:
             pass
 
 
@@ -742,15 +766,15 @@
                 "The `connection_pool_limits` argument is deprecated. The `http_client` argument should be passed instead",
                 category=DeprecationWarning,
                 stacklevel=3,
             )
             if http_client is not None:
                 raise ValueError("The `http_client` argument is mutually exclusive with `connection_pool_limits`")
         else:
-            limits = DEFAULT_LIMITS
+            limits = DEFAULT_CONNECTION_LIMITS
 
         if transport is not None:
             warnings.warn(
                 "The `transport` argument is deprecated. The `http_client` argument should be passed instead",
                 category=DeprecationWarning,
                 stacklevel=3,
             )
@@ -917,14 +941,16 @@
         request = self._build_request(options)
         self._prepare_request(request)
 
         kwargs: HttpxSendArgs = {}
         if self.custom_auth is not None:
             kwargs["auth"] = self.custom_auth
 
+        log.debug("Sending HTTP Request: %s %s", request.method, request.url)
+
         try:
             response = self._client.send(
                 request,
                 stream=stream or self._should_stream_response_body(request=request),
                 **kwargs,
             )
         except httpx.TimeoutException as err:
@@ -955,15 +981,20 @@
                     response_headers=None,
                 )
 
             log.debug("Raising connection error")
             raise APIConnectionError(request=request) from err
 
         log.debug(
-            'HTTP Request: %s %s "%i %s"', request.method, request.url, response.status_code, response.reason_phrase
+            'HTTP Response: %s %s "%i %s" %s',
+            request.method,
+            request.url,
+            response.status_code,
+            response.reason_phrase,
+            response.headers,
         )
 
         try:
             response.raise_for_status()
         except httpx.HTTPStatusError as err:  # thrown on 4xx and 5xx status code
             log.debug("Encountered httpx.HTTPStatusError", exc_info=True)
 
@@ -1239,15 +1270,35 @@
         options: RequestOptions = {},
         method: str = "get",
     ) -> SyncPageT:
         opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
         return self._request_api_list(model, page, opts)
 
 
-class AsyncHttpxClientWrapper(httpx.AsyncClient):
+class _DefaultAsyncHttpxClient(httpx.AsyncClient):
+    def __init__(self, **kwargs: Any) -> None:
+        kwargs.setdefault("timeout", DEFAULT_TIMEOUT)
+        kwargs.setdefault("limits", DEFAULT_CONNECTION_LIMITS)
+        kwargs.setdefault("follow_redirects", True)
+        super().__init__(**kwargs)
+
+
+if TYPE_CHECKING:
+    DefaultAsyncHttpxClient = httpx.AsyncClient
+    """An alias to `httpx.AsyncClient` that provides the same defaults that this SDK
+    uses internally.
+
+    This is useful because overriding the `http_client` with your own instance of
+    `httpx.AsyncClient` will result in httpx's defaults being used, not ours.
+    """
+else:
+    DefaultAsyncHttpxClient = _DefaultAsyncHttpxClient
+
+
+class AsyncHttpxClientWrapper(DefaultAsyncHttpxClient):
     def __del__(self) -> None:
         try:
             # TODO(someday): support non asyncio runtimes here
             asyncio.get_running_loop().create_task(self.aclose())
         except Exception:
             pass
 
@@ -1276,15 +1327,15 @@
                 "The `connection_pool_limits` argument is deprecated. The `http_client` argument should be passed instead",
                 category=DeprecationWarning,
                 stacklevel=3,
             )
             if http_client is not None:
                 raise ValueError("The `http_client` argument is mutually exclusive with `connection_pool_limits`")
         else:
-            limits = DEFAULT_LIMITS
+            limits = DEFAULT_CONNECTION_LIMITS
 
         if transport is not None:
             warnings.warn(
                 "The `transport` argument is deprecated. The `http_client` argument should be passed instead",
                 category=DeprecationWarning,
                 stacklevel=3,
             )
```

### Comparing `groq-0.5.0/src/groq/_client.py` & `groq-0.6.0/src/groq/_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import os
 from typing import Any, Union, Mapping
 from typing_extensions import Self, override
 
@@ -42,14 +42,15 @@
     "AsyncGroq",
     "Client",
     "AsyncClient",
 ]
 
 
 class Groq(SyncAPIClient):
+    embeddings: resources.Embeddings
     chat: resources.Chat
     audio: resources.Audio
     models: resources.Models
     with_raw_response: GroqWithRawResponse
     with_streaming_response: GroqWithStreamedResponse
 
     # client options
@@ -60,15 +61,17 @@
         *,
         api_key: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
-        # Configure a custom httpx client. See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
+        # Configure a custom httpx client.
+        # We provide a `DefaultHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
+        # See the [httpx documentation](https://www.python-httpx.org/api/#client) for more details.
         http_client: httpx.Client | None = None,
         # Enable or disable schema validation for data returned by the API.
         # When enabled an error APIResponseValidationError is raised
         # if the API responds with invalid data for the expected schema.
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
@@ -100,14 +103,15 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
+        self.embeddings = resources.Embeddings(self)
         self.chat = resources.Chat(self)
         self.audio = resources.Audio(self)
         self.models = resources.Models(self)
         self.with_raw_response = GroqWithRawResponse(self)
         self.with_streaming_response = GroqWithStreamedResponse(self)
 
     @property
@@ -212,14 +216,15 @@
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class AsyncGroq(AsyncAPIClient):
+    embeddings: resources.AsyncEmbeddings
     chat: resources.AsyncChat
     audio: resources.AsyncAudio
     models: resources.AsyncModels
     with_raw_response: AsyncGroqWithRawResponse
     with_streaming_response: AsyncGroqWithStreamedResponse
 
     # client options
@@ -230,15 +235,17 @@
         *,
         api_key: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
-        # Configure a custom httpx client. See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
+        # Configure a custom httpx client.
+        # We provide a `DefaultAsyncHttpxClient` class that you can pass to retain the default values we use for `limits`, `timeout` & `follow_redirects`.
+        # See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
         http_client: httpx.AsyncClient | None = None,
         # Enable or disable schema validation for data returned by the API.
         # When enabled an error APIResponseValidationError is raised
         # if the API responds with invalid data for the expected schema.
         #
         # This parameter may be removed or changed in the future.
         # If you rely on this feature, please open a GitHub issue
@@ -270,14 +277,15 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
+        self.embeddings = resources.AsyncEmbeddings(self)
         self.chat = resources.AsyncChat(self)
         self.audio = resources.AsyncAudio(self)
         self.models = resources.AsyncModels(self)
         self.with_raw_response = AsyncGroqWithRawResponse(self)
         self.with_streaming_response = AsyncGroqWithStreamedResponse(self)
 
     @property
@@ -383,35 +391,39 @@
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class GroqWithRawResponse:
     def __init__(self, client: Groq) -> None:
+        self.embeddings = resources.EmbeddingsWithRawResponse(client.embeddings)
         self.chat = resources.ChatWithRawResponse(client.chat)
         self.audio = resources.AudioWithRawResponse(client.audio)
         self.models = resources.ModelsWithRawResponse(client.models)
 
 
 class AsyncGroqWithRawResponse:
     def __init__(self, client: AsyncGroq) -> None:
+        self.embeddings = resources.AsyncEmbeddingsWithRawResponse(client.embeddings)
         self.chat = resources.AsyncChatWithRawResponse(client.chat)
         self.audio = resources.AsyncAudioWithRawResponse(client.audio)
         self.models = resources.AsyncModelsWithRawResponse(client.models)
 
 
 class GroqWithStreamedResponse:
     def __init__(self, client: Groq) -> None:
+        self.embeddings = resources.EmbeddingsWithStreamingResponse(client.embeddings)
         self.chat = resources.ChatWithStreamingResponse(client.chat)
         self.audio = resources.AudioWithStreamingResponse(client.audio)
         self.models = resources.ModelsWithStreamingResponse(client.models)
 
 
 class AsyncGroqWithStreamedResponse:
     def __init__(self, client: AsyncGroq) -> None:
+        self.embeddings = resources.AsyncEmbeddingsWithStreamingResponse(client.embeddings)
         self.chat = resources.AsyncChatWithStreamingResponse(client.chat)
         self.audio = resources.AsyncAudioWithStreamingResponse(client.audio)
         self.models = resources.AsyncModelsWithStreamingResponse(client.models)
 
 
 Client = Groq
```

### Comparing `groq-0.5.0/src/groq/_compat.py` & `groq-0.6.0/src/groq/_compat.py`

 * *Files identical despite different names*

### Comparing `groq-0.5.0/src/groq/_exceptions.py` & `groq-0.6.0/src/groq/_exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing_extensions import Literal
 
 import httpx
```

### Comparing `groq-0.5.0/src/groq/_files.py` & `groq-0.6.0/src/groq/_files.py`

 * *Files identical despite different names*

### Comparing `groq-0.5.0/src/groq/_models.py` & `groq-0.6.0/src/groq/_models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
+import os
 import inspect
 from typing import TYPE_CHECKING, Any, Type, Union, Generic, TypeVar, Callable, cast
 from datetime import date, datetime
 from typing_extensions import (
     Unpack,
     Literal,
     ClassVar,
     Protocol,
     Required,
     TypedDict,
+    TypeGuard,
     final,
     override,
     runtime_checkable,
 )
 
 import pydantic
 import pydantic.generics
@@ -26,15 +28,28 @@
     ModelT,
     Headers,
     Timeout,
     NotGiven,
     AnyMapping,
     HttpxRequestFiles,
 )
-from ._utils import is_list, is_given, is_mapping, parse_date, parse_datetime, strip_not_given
+from ._utils import (
+    PropertyInfo,
+    is_list,
+    is_given,
+    lru_cache,
+    is_mapping,
+    parse_date,
+    coerce_boolean,
+    parse_datetime,
+    strip_not_given,
+    extract_type_arg,
+    is_annotated_type,
+    strip_annotated_type,
+)
 from ._compat import (
     PYDANTIC_V2,
     ConfigDict,
     GenericModel as BaseGenericModel,
     get_args,
     is_union,
     parse_obj,
@@ -42,38 +57,116 @@
     is_literal_type,
     get_model_config,
     get_model_fields,
     field_get_default,
 )
 from ._constants import RAW_RESPONSE_HEADER
 
+if TYPE_CHECKING:
+    from pydantic_core.core_schema import ModelField, LiteralSchema, ModelFieldsSchema
+
 __all__ = ["BaseModel", "GenericModel"]
 
 _T = TypeVar("_T")
 
 
 @runtime_checkable
 class _ConfigProtocol(Protocol):
     allow_population_by_field_name: bool
 
 
 class BaseModel(pydantic.BaseModel):
     if PYDANTIC_V2:
-        model_config: ClassVar[ConfigDict] = ConfigDict(extra="allow")
+        model_config: ClassVar[ConfigDict] = ConfigDict(
+            extra="allow", defer_build=coerce_boolean(os.environ.get("DEFER_PYDANTIC_BUILD", "true"))
+        )
     else:
 
         @property
         @override
         def model_fields_set(self) -> set[str]:
             # a forwards-compat shim for pydantic v2
             return self.__fields_set__  # type: ignore
 
         class Config(pydantic.BaseConfig):  # pyright: ignore[reportDeprecated]
             extra: Any = pydantic.Extra.allow  # type: ignore
 
+    def to_dict(
+        self,
+        *,
+        mode: Literal["json", "python"] = "python",
+        use_api_names: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        warnings: bool = True,
+    ) -> dict[str, object]:
+        """Recursively generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
+
+        By default, fields that were not set by the API will not be included,
+        and keys will match the API response, *not* the property names from the model.
+
+        For example, if the API responds with `"fooBar": true` but we've defined a `foo_bar: bool` property,
+        the output will use the `"fooBar"` key (unless `use_api_names=False` is passed).
+
+        Args:
+            mode:
+                If mode is 'json', the dictionary will only contain JSON serializable types. e.g. `datetime` will be turned into a string, `"2024-3-22T18:11:19.117000Z"`.
+                If mode is 'python', the dictionary may contain any Python objects. e.g. `datetime(2024, 3, 22)`
+
+            use_api_names: Whether to use the key that the API responded with or the property name. Defaults to `True`.
+            exclude_unset: Whether to exclude fields that have not been explicitly set.
+            exclude_defaults: Whether to exclude fields that are set to their default value from the output.
+            exclude_none: Whether to exclude fields that have a value of `None` from the output.
+            warnings: Whether to log warnings when invalid fields are encountered. This is only supported in Pydantic v2.
+        """
+        return self.model_dump(
+            mode=mode,
+            by_alias=use_api_names,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            warnings=warnings,
+        )
+
+    def to_json(
+        self,
+        *,
+        indent: int | None = 2,
+        use_api_names: bool = True,
+        exclude_unset: bool = True,
+        exclude_defaults: bool = False,
+        exclude_none: bool = False,
+        warnings: bool = True,
+    ) -> str:
+        """Generates a JSON string representing this model as it would be received from or sent to the API (but with indentation).
+
+        By default, fields that were not set by the API will not be included,
+        and keys will match the API response, *not* the property names from the model.
+
+        For example, if the API responds with `"fooBar": true` but we've defined a `foo_bar: bool` property,
+        the output will use the `"fooBar"` key (unless `use_api_names=False` is passed).
+
+        Args:
+            indent: Indentation to use in the JSON output. If `None` is passed, the output will be compact. Defaults to `2`
+            use_api_names: Whether to use the key that the API responded with or the property name. Defaults to `True`.
+            exclude_unset: Whether to exclude fields that have not been explicitly set.
+            exclude_defaults: Whether to exclude fields that have the default value.
+            exclude_none: Whether to exclude fields that have a value of `None`.
+            warnings: Whether to show any warnings that occurred during serialization. This is only supported in Pydantic v2.
+        """
+        return self.model_dump_json(
+            indent=indent,
+            by_alias=use_api_names,
+            exclude_unset=exclude_unset,
+            exclude_defaults=exclude_defaults,
+            exclude_none=exclude_none,
+            warnings=warnings,
+        )
+
     @override
     def __str__(self) -> str:
         # mypy complains about an invalid self arg
         return f'{self.__repr_name__()}({self.__repr_str__(", ")})'  # type: ignore[misc]
 
     # Override the 'construct' method in a way that supports recursive parsing without validation.
     # Based on https://github.com/samuelcolvin/pydantic/issues/1168#issuecomment-817742836.
@@ -154,15 +247,17 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool = True,
+            warnings: bool | Literal["none", "warn", "error"] = True,
+            context: dict[str, Any] | None = None,
+            serialize_as_any: bool = False,
         ) -> dict[str, Any]:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump
 
             Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
 
             Args:
                 mode: The mode in which `to_python` should run.
@@ -182,14 +277,18 @@
             """
             if mode != "python":
                 raise ValueError("mode is only supported in Pydantic v2")
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
+            if context is not None:
+                raise ValueError("context is only supported in Pydantic v2")
+            if serialize_as_any != False:
+                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().dict(  # pyright: ignore[reportDeprecated]
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
                 exclude_none=exclude_none,
@@ -203,15 +302,17 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool = True,
+            warnings: bool | Literal["none", "warn", "error"] = True,
+            context: dict[str, Any] | None = None,
+            serialize_as_any: bool = False,
         ) -> str:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump_json
 
             Generates a JSON representation of the model using Pydantic's `to_json` method.
 
             Args:
                 indent: Indentation to use in the JSON output. If None is passed, the output will be compact.
@@ -227,14 +328,18 @@
             Returns:
                 A JSON string representation of the model.
             """
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
+            if context is not None:
+                raise ValueError("context is only supported in Pydantic v2")
+            if serialize_as_any != False:
+                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().json(  # type: ignore[reportDeprecated]
                 indent=indent,
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
@@ -255,42 +360,78 @@
         raise RuntimeError(f"Unexpected field type is None for {key}")
 
     return construct_type(value=value, type_=type_)
 
 
 def is_basemodel(type_: type) -> bool:
     """Returns whether or not the given type is either a `BaseModel` or a union of `BaseModel`"""
-    origin = get_origin(type_) or type_
     if is_union(type_):
         for variant in get_args(type_):
             if is_basemodel(variant):
                 return True
 
         return False
 
+    return is_basemodel_type(type_)
+
+
+def is_basemodel_type(type_: type) -> TypeGuard[type[BaseModel] | type[GenericModel]]:
+    origin = get_origin(type_) or type_
     return issubclass(origin, BaseModel) or issubclass(origin, GenericModel)
 
 
-def construct_type(*, value: object, type_: type) -> object:
+def construct_type(*, value: object, type_: object) -> object:
     """Loose coercion to the expected type with construction of nested values.
 
     If the given value does not match the expected type then it is returned as-is.
     """
+    # we allow `object` as the input type because otherwise, passing things like
+    # `Literal['value']` will be reported as a type error by type checkers
+    type_ = cast("type[object]", type_)
+
+    # unwrap `Annotated[T, ...]` -> `T`
+    if is_annotated_type(type_):
+        meta: tuple[Any, ...] = get_args(type_)[1:]
+        type_ = extract_type_arg(type_, 0)
+    else:
+        meta = tuple()
 
     # we need to use the origin class for any types that are subscripted generics
     # e.g. Dict[str, object]
     origin = get_origin(type_) or type_
     args = get_args(type_)
 
     if is_union(origin):
         try:
             return validate_type(type_=cast("type[object]", type_), value=value)
         except Exception:
             pass
 
+        # if the type is a discriminated union then we want to construct the right variant
+        # in the union, even if the data doesn't match exactly, otherwise we'd break code
+        # that relies on the constructed class types, e.g.
+        #
+        # class FooType:
+        #   kind: Literal['foo']
+        #   value: str
+        #
+        # class BarType:
+        #   kind: Literal['bar']
+        #   value: int
+        #
+        # without this block, if the data we get is something like `{'kind': 'bar', 'value': 'foo'}` then
+        # we'd end up constructing `FooType` when it should be `BarType`.
+        discriminator = _build_discriminated_union_meta(union=type_, meta_annotations=meta)
+        if discriminator and is_mapping(value):
+            variant_value = value.get(discriminator.field_alias_from or discriminator.field_name)
+            if variant_value and isinstance(variant_value, str):
+                variant_type = discriminator.mapping.get(variant_value)
+                if variant_type:
+                    return construct_type(type_=variant_type, value=value)
+
         # if the data is not valid, use the first variant that doesn't fail while deserializing
         for variant in args:
             try:
                 return construct_type(value=value, type_=variant)
             except Exception:
                 continue
 
@@ -340,14 +481,137 @@
             return parse_date(value)  # type: ignore
         except Exception:
             return value
 
     return value
 
 
+@runtime_checkable
+class CachedDiscriminatorType(Protocol):
+    __discriminator__: DiscriminatorDetails
+
+
+class DiscriminatorDetails:
+    field_name: str
+    """The name of the discriminator field in the variant class, e.g.
+
+    ```py
+    class Foo(BaseModel):
+        type: Literal['foo']
+    ```
+
+    Will result in field_name='type'
+    """
+
+    field_alias_from: str | None
+    """The name of the discriminator field in the API response, e.g.
+
+    ```py
+    class Foo(BaseModel):
+        type: Literal['foo'] = Field(alias='type_from_api')
+    ```
+
+    Will result in field_alias_from='type_from_api'
+    """
+
+    mapping: dict[str, type]
+    """Mapping of discriminator value to variant type, e.g.
+
+    {'foo': FooVariant, 'bar': BarVariant}
+    """
+
+    def __init__(
+        self,
+        *,
+        mapping: dict[str, type],
+        discriminator_field: str,
+        discriminator_alias: str | None,
+    ) -> None:
+        self.mapping = mapping
+        self.field_name = discriminator_field
+        self.field_alias_from = discriminator_alias
+
+
+def _build_discriminated_union_meta(*, union: type, meta_annotations: tuple[Any, ...]) -> DiscriminatorDetails | None:
+    if isinstance(union, CachedDiscriminatorType):
+        return union.__discriminator__
+
+    discriminator_field_name: str | None = None
+
+    for annotation in meta_annotations:
+        if isinstance(annotation, PropertyInfo) and annotation.discriminator is not None:
+            discriminator_field_name = annotation.discriminator
+            break
+
+    if not discriminator_field_name:
+        return None
+
+    mapping: dict[str, type] = {}
+    discriminator_alias: str | None = None
+
+    for variant in get_args(union):
+        variant = strip_annotated_type(variant)
+        if is_basemodel_type(variant):
+            if PYDANTIC_V2:
+                field = _extract_field_schema_pv2(variant, discriminator_field_name)
+                if not field:
+                    continue
+
+                # Note: if one variant defines an alias then they all should
+                discriminator_alias = field.get("serialization_alias")
+
+                field_schema = field["schema"]
+
+                if field_schema["type"] == "literal":
+                    for entry in cast("LiteralSchema", field_schema)["expected"]:
+                        if isinstance(entry, str):
+                            mapping[entry] = variant
+            else:
+                field_info = cast("dict[str, FieldInfo]", variant.__fields__).get(discriminator_field_name)  # pyright: ignore[reportDeprecated, reportUnnecessaryCast]
+                if not field_info:
+                    continue
+
+                # Note: if one variant defines an alias then they all should
+                discriminator_alias = field_info.alias
+
+                if field_info.annotation and is_literal_type(field_info.annotation):
+                    for entry in get_args(field_info.annotation):
+                        if isinstance(entry, str):
+                            mapping[entry] = variant
+
+    if not mapping:
+        return None
+
+    details = DiscriminatorDetails(
+        mapping=mapping,
+        discriminator_field=discriminator_field_name,
+        discriminator_alias=discriminator_alias,
+    )
+    cast(CachedDiscriminatorType, union).__discriminator__ = details
+    return details
+
+
+def _extract_field_schema_pv2(model: type[BaseModel], field_name: str) -> ModelField | None:
+    schema = model.__pydantic_core_schema__
+    if schema["type"] != "model":
+        return None
+
+    fields_schema = schema["schema"]
+    if fields_schema["type"] != "model-fields":
+        return None
+
+    fields_schema = cast("ModelFieldsSchema", fields_schema)
+
+    field = fields_schema["fields"].get(field_name)
+    if not field:
+        return None
+
+    return cast("ModelField", field)  # pyright: ignore[reportUnnecessaryCast]
+
+
 def validate_type(*, type_: type[_T], value: object) -> _T:
     """Strict validation that the given value matches the expected type"""
     if inspect.isclass(type_) and issubclass(type_, pydantic.BaseModel):
         return cast(_T, parse_obj(type_, value))
 
     return cast(_T, _validate_non_model_type(type_=type_, value=value))
 
@@ -359,15 +623,22 @@
 else:
 
     class GenericModel(BaseGenericModel, BaseModel):
         pass
 
 
 if PYDANTIC_V2:
-    from pydantic import TypeAdapter
+    from pydantic import TypeAdapter as _TypeAdapter
+
+    _CachedTypeAdapter = cast("TypeAdapter[object]", lru_cache(maxsize=None)(_TypeAdapter))
+
+    if TYPE_CHECKING:
+        from pydantic import TypeAdapter
+    else:
+        TypeAdapter = _CachedTypeAdapter
 
     def _validate_non_model_type(*, type_: type[_T], value: object) -> _T:
         return TypeAdapter(type_).validate_python(value)
 
 elif not TYPE_CHECKING:  # TODO: condition is weird
 
     class RootModel(GenericModel, Generic[_T]):
```

### Comparing `groq-0.5.0/src/groq/_qs.py` & `groq-0.6.0/src/groq/_qs.py`

 * *Files identical despite different names*

### Comparing `groq-0.5.0/src/groq/_resource.py` & `groq-0.6.0/src/groq/_resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import time
 from typing import TYPE_CHECKING
 
 import anyio
```

### Comparing `groq-0.5.0/src/groq/_response.py` & `groq-0.6.0/src/groq/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from typing_extensions import Awaitable, ParamSpec, override, get_origin
 
 import anyio
 import httpx
 import pydantic
 
 from ._types import NoneType
-from ._utils import is_given, extract_type_var_from_base
+from ._utils import is_given, extract_type_arg, is_annotated_type, extract_type_var_from_base
 from ._models import BaseModel, is_basemodel
 from ._constants import RAW_RESPONSE_HEADER, OVERRIDE_CAST_TO_HEADER
 from ._streaming import Stream, AsyncStream, is_stream_class_type, extract_stream_chunk_type
 from ._exceptions import GroqError, APIResponseValidationError
 
 if TYPE_CHECKING:
     from ._models import FinalRequestOptions
@@ -117,14 +117,18 @@
     @override
     def __repr__(self) -> str:
         return (
             f"<{self.__class__.__name__} [{self.status_code} {self.http_response.reason_phrase}] type={self._cast_to}>"
         )
 
     def _parse(self, *, to: type[_T] | None = None) -> R | _T:
+        # unwrap `Annotated[T, ...]` -> `T`
+        if to and is_annotated_type(to):
+            to = extract_type_arg(to, 0)
+
         if self._is_sse_stream:
             if to:
                 if not is_stream_class_type(to):
                     raise TypeError(f"Expected custom parse type to be a subclass of {Stream} or {AsyncStream}")
 
                 return cast(
                     _T,
@@ -158,14 +162,19 @@
                     cast_to=self._cast_to,
                     response=self.http_response,
                     client=cast(Any, self._client),
                 ),
             )
 
         cast_to = to if to is not None else self._cast_to
+
+        # unwrap `Annotated[T, ...]` -> `T`
+        if is_annotated_type(cast_to):
+            cast_to = extract_type_arg(cast_to, 0)
+
         if cast_to is NoneType:
             return cast(R, None)
 
         response = self.http_response
         if cast_to == str:
             return cast(R, response.text)
 
@@ -626,15 +635,15 @@
 def to_streamed_response_wrapper(func: Callable[P, R]) -> Callable[P, ResponseContextManager[APIResponse[R]]]:
     """Higher order function that takes one of our bound API methods and wraps it
     to support streaming and returning the raw `APIResponse` object directly.
     """
 
     @functools.wraps(func)
     def wrapped(*args: P.args, **kwargs: P.kwargs) -> ResponseContextManager[APIResponse[R]]:
-        extra_headers = {**(cast(Any, kwargs.get("extra_headers")) or {})}
+        extra_headers: dict[str, str] = {**(cast(Any, kwargs.get("extra_headers")) or {})}
         extra_headers[RAW_RESPONSE_HEADER] = "stream"
 
         kwargs["extra_headers"] = extra_headers
 
         make_request = functools.partial(func, *args, **kwargs)
 
         return ResponseContextManager(cast(Callable[[], APIResponse[R]], make_request))
@@ -647,15 +656,15 @@
 ) -> Callable[P, AsyncResponseContextManager[AsyncAPIResponse[R]]]:
     """Higher order function that takes one of our bound API methods and wraps it
     to support streaming and returning the raw `APIResponse` object directly.
     """
 
     @functools.wraps(func)
     def wrapped(*args: P.args, **kwargs: P.kwargs) -> AsyncResponseContextManager[AsyncAPIResponse[R]]:
-        extra_headers = {**(cast(Any, kwargs.get("extra_headers")) or {})}
+        extra_headers: dict[str, str] = {**(cast(Any, kwargs.get("extra_headers")) or {})}
         extra_headers[RAW_RESPONSE_HEADER] = "stream"
 
         kwargs["extra_headers"] = extra_headers
 
         make_request = func(*args, **kwargs)
 
         return AsyncResponseContextManager(cast(Awaitable[AsyncAPIResponse[R]], make_request))
@@ -671,15 +680,15 @@
     and wraps the method to support streaming and returning the given response class directly.
 
     Note: the given `response_cls` *must* be concrete, e.g. `class BinaryAPIResponse(APIResponse[bytes])`
     """
 
     @functools.wraps(func)
     def wrapped(*args: P.args, **kwargs: P.kwargs) -> ResponseContextManager[_APIResponseT]:
-        extra_headers = {**(cast(Any, kwargs.get("extra_headers")) or {})}
+        extra_headers: dict[str, Any] = {**(cast(Any, kwargs.get("extra_headers")) or {})}
         extra_headers[RAW_RESPONSE_HEADER] = "stream"
         extra_headers[OVERRIDE_CAST_TO_HEADER] = response_cls
 
         kwargs["extra_headers"] = extra_headers
 
         make_request = functools.partial(func, *args, **kwargs)
 
@@ -696,15 +705,15 @@
     and wraps the method to support streaming and returning the given response class directly.
 
     Note: the given `response_cls` *must* be concrete, e.g. `class BinaryAPIResponse(APIResponse[bytes])`
     """
 
     @functools.wraps(func)
     def wrapped(*args: P.args, **kwargs: P.kwargs) -> AsyncResponseContextManager[_AsyncAPIResponseT]:
-        extra_headers = {**(cast(Any, kwargs.get("extra_headers")) or {})}
+        extra_headers: dict[str, Any] = {**(cast(Any, kwargs.get("extra_headers")) or {})}
         extra_headers[RAW_RESPONSE_HEADER] = "stream"
         extra_headers[OVERRIDE_CAST_TO_HEADER] = response_cls
 
         kwargs["extra_headers"] = extra_headers
 
         make_request = func(*args, **kwargs)
 
@@ -716,15 +725,15 @@
 def to_raw_response_wrapper(func: Callable[P, R]) -> Callable[P, APIResponse[R]]:
     """Higher order function that takes one of our bound API methods and wraps it
     to support returning the raw `APIResponse` object directly.
     """
 
     @functools.wraps(func)
     def wrapped(*args: P.args, **kwargs: P.kwargs) -> APIResponse[R]:
-        extra_headers = {**(cast(Any, kwargs.get("extra_headers")) or {})}
+        extra_headers: dict[str, str] = {**(cast(Any, kwargs.get("extra_headers")) or {})}
         extra_headers[RAW_RESPONSE_HEADER] = "raw"
 
         kwargs["extra_headers"] = extra_headers
 
         return cast(APIResponse[R], func(*args, **kwargs))
 
     return wrapped
@@ -733,15 +742,15 @@
 def async_to_raw_response_wrapper(func: Callable[P, Awaitable[R]]) -> Callable[P, Awaitable[AsyncAPIResponse[R]]]:
     """Higher order function that takes one of our bound API methods and wraps it
     to support returning the raw `APIResponse` object directly.
     """
 
     @functools.wraps(func)
     async def wrapped(*args: P.args, **kwargs: P.kwargs) -> AsyncAPIResponse[R]:
-        extra_headers = {**(cast(Any, kwargs.get("extra_headers")) or {})}
+        extra_headers: dict[str, str] = {**(cast(Any, kwargs.get("extra_headers")) or {})}
         extra_headers[RAW_RESPONSE_HEADER] = "raw"
 
         kwargs["extra_headers"] = extra_headers
 
         return cast(AsyncAPIResponse[R], await func(*args, **kwargs))
 
     return wrapped
@@ -755,15 +764,15 @@
     and wraps the method to support returning the given response class directly.
 
     Note: the given `response_cls` *must* be concrete, e.g. `class BinaryAPIResponse(APIResponse[bytes])`
     """
 
     @functools.wraps(func)
     def wrapped(*args: P.args, **kwargs: P.kwargs) -> _APIResponseT:
-        extra_headers = {**(cast(Any, kwargs.get("extra_headers")) or {})}
+        extra_headers: dict[str, Any] = {**(cast(Any, kwargs.get("extra_headers")) or {})}
         extra_headers[RAW_RESPONSE_HEADER] = "raw"
         extra_headers[OVERRIDE_CAST_TO_HEADER] = response_cls
 
         kwargs["extra_headers"] = extra_headers
 
         return cast(_APIResponseT, func(*args, **kwargs))
 
@@ -778,15 +787,15 @@
     and wraps the method to support returning the given response class directly.
 
     Note: the given `response_cls` *must* be concrete, e.g. `class BinaryAPIResponse(APIResponse[bytes])`
     """
 
     @functools.wraps(func)
     def wrapped(*args: P.args, **kwargs: P.kwargs) -> Awaitable[_AsyncAPIResponseT]:
-        extra_headers = {**(cast(Any, kwargs.get("extra_headers")) or {})}
+        extra_headers: dict[str, Any] = {**(cast(Any, kwargs.get("extra_headers")) or {})}
         extra_headers[RAW_RESPONSE_HEADER] = "raw"
         extra_headers[OVERRIDE_CAST_TO_HEADER] = response_cls
 
         kwargs["extra_headers"] = extra_headers
 
         return cast(Awaitable[_AsyncAPIResponseT], func(*args, **kwargs))
```

### Comparing `groq-0.5.0/src/groq/_streaming.py` & `groq-0.6.0/src/groq/_streaming.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class Stream(Generic[_T]):
     """Provides the core interface to iterate over a synchronous stream response."""
 
     response: httpx.Response
 
-    _decoder: SSEDecoder | SSEBytesDecoder
+    _decoder: SSEBytesDecoder
 
     def __init__(
         self,
         *,
         cast_to: type[_T],
         response: httpx.Response,
         client: Groq,
@@ -42,18 +42,15 @@
         return self._iterator.__next__()
 
     def __iter__(self) -> Iterator[_T]:
         for item in self._iterator:
             yield item
 
     def _iter_events(self) -> Iterator[ServerSentEvent]:
-        if isinstance(self._decoder, SSEBytesDecoder):
-            yield from self._decoder.iter_bytes(self.response.iter_bytes())
-        else:
-            yield from self._decoder.iter(self.response.iter_lines())
+        yield from self._decoder.iter_bytes(self.response.iter_bytes())
 
     def __stream__(self) -> Iterator[_T]:
         cast_to = cast(Any, self._cast_to)
         response = self.response
         process_data = self._client._process_response_data
         iterator = self._iter_events()
 
@@ -110,32 +107,26 @@
         return await self._iterator.__anext__()
 
     async def __aiter__(self) -> AsyncIterator[_T]:
         async for item in self._iterator:
             yield item
 
     async def _iter_events(self) -> AsyncIterator[ServerSentEvent]:
-        if isinstance(self._decoder, SSEBytesDecoder):
-            async for sse in self._decoder.aiter_bytes(self.response.aiter_bytes()):
-                if sse.data.startswith("[DONE]"):
-                    break
-                yield sse
-        else:
-            async for sse in self._decoder.aiter(self.response.aiter_lines()):
-                if sse.data.startswith("[DONE]"):
-                    break
-                yield sse
+        async for sse in self._decoder.aiter_bytes(self.response.aiter_bytes()):
+            yield sse
 
     async def __stream__(self) -> AsyncIterator[_T]:
         cast_to = cast(Any, self._cast_to)
         response = self.response
         process_data = self._client._process_response_data
         iterator = self._iter_events()
 
         async for sse in iterator:
+            if sse.data.startswith("[DONE]"):
+                break
             yield process_data(data=sse.json(), cast_to=cast_to, response=response)
 
         # Ensure the entire stream is consumed
         async for _sse in iterator:
             ...
 
     async def __aenter__(self) -> Self:
@@ -207,29 +198,57 @@
 
     def __init__(self) -> None:
         self._event = None
         self._data = []
         self._last_event_id = None
         self._retry = None
 
-    def iter(self, iterator: Iterator[str]) -> Iterator[ServerSentEvent]:
-        """Given an iterator that yields lines, iterate over it & yield every event encountered"""
-        for line in iterator:
-            line = line.rstrip("\n")
-            sse = self.decode(line)
-            if sse is not None:
-                yield sse
-
-    async def aiter(self, iterator: AsyncIterator[str]) -> AsyncIterator[ServerSentEvent]:
-        """Given an async iterator that yields lines, iterate over it & yield every event encountered"""
-        async for line in iterator:
-            line = line.rstrip("\n")
-            sse = self.decode(line)
-            if sse is not None:
-                yield sse
+    def iter_bytes(self, iterator: Iterator[bytes]) -> Iterator[ServerSentEvent]:
+        """Given an iterator that yields raw binary data, iterate over it & yield every event encountered"""
+        for chunk in self._iter_chunks(iterator):
+            # Split before decoding so splitlines() only uses \r and \n
+            for raw_line in chunk.splitlines():
+                line = raw_line.decode("utf-8")
+                sse = self.decode(line)
+                if sse:
+                    yield sse
+
+    def _iter_chunks(self, iterator: Iterator[bytes]) -> Iterator[bytes]:
+        """Given an iterator that yields raw binary data, iterate over it and yield individual SSE chunks"""
+        data = b""
+        for chunk in iterator:
+            for line in chunk.splitlines(keepends=True):
+                data += line
+                if data.endswith((b"\r\r", b"\n\n", b"\r\n\r\n")):
+                    yield data
+                    data = b""
+        if data:
+            yield data
+
+    async def aiter_bytes(self, iterator: AsyncIterator[bytes]) -> AsyncIterator[ServerSentEvent]:
+        """Given an iterator that yields raw binary data, iterate over it & yield every event encountered"""
+        async for chunk in self._aiter_chunks(iterator):
+            # Split before decoding so splitlines() only uses \r and \n
+            for raw_line in chunk.splitlines():
+                line = raw_line.decode("utf-8")
+                sse = self.decode(line)
+                if sse:
+                    yield sse
+
+    async def _aiter_chunks(self, iterator: AsyncIterator[bytes]) -> AsyncIterator[bytes]:
+        """Given an iterator that yields raw binary data, iterate over it and yield individual SSE chunks"""
+        data = b""
+        async for chunk in iterator:
+            for line in chunk.splitlines(keepends=True):
+                data += line
+                if data.endswith((b"\r\r", b"\n\n", b"\r\n\r\n")):
+                    yield data
+                    data = b""
+        if data:
+            yield data
 
     def decode(self, line: str) -> ServerSentEvent | None:
         # See: https://html.spec.whatwg.org/multipage/server-sent-events.html#event-stream-interpretation  # noqa: E501
 
         if not line:
             if not self._event and not self._data and not self._last_event_id and self._retry is None:
                 return None
```

### Comparing `groq-0.5.0/src/groq/_types.py` & `groq-0.6.0/src/groq/_types.py`

 * *Files identical despite different names*

### Comparing `groq-0.5.0/src/groq/_utils/__init__.py` & `groq-0.6.0/src/groq/_utils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ._proxy import LazyProxy as LazyProxy
 from ._utils import (
     flatten as flatten,
     is_dict as is_dict,
     is_list as is_list,
     is_given as is_given,
     is_tuple as is_tuple,
+    lru_cache as lru_cache,
     is_mapping as is_mapping,
     is_tuple_t as is_tuple_t,
     parse_date as parse_date,
     is_iterable as is_iterable,
     is_sequence as is_sequence,
     coerce_float as coerce_float,
     is_mapping_t as is_mapping_t,
```

### Comparing `groq-0.5.0/src/groq/_utils/_logs.py` & `groq-0.6.0/src/groq/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `groq-0.5.0/src/groq/_utils/_proxy.py` & `groq-0.6.0/src/groq/_utils/_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 T = TypeVar("T")
 
 
 class LazyProxy(Generic[T], ABC):
     """Implements data methods to pretend that an instance is another instance.
 
-    This includes forwarding attribute access and othe methods.
+    This includes forwarding attribute access and other methods.
     """
 
     # Note: we have to special case proxies that themselves return proxies
     # to support using a proxy as a catch-all for any random access, e.g. `proxy.foo.bar.baz`
 
     def __getattr__(self, attr: str) -> object:
         proxied = self.__get_proxied__()
```

### Comparing `groq-0.5.0/src/groq/_utils/_sync.py` & `groq-0.6.0/src/groq/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `groq-0.5.0/src/groq/_utils/_transform.py` & `groq-0.6.0/src/groq/_utils/_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,29 +47,32 @@
 
     This means that {'account_holder_name': 'Robert'} will be transformed to {'accountHolderName': 'Robert'} before being sent to the API.
     """
 
     alias: str | None
     format: PropertyFormat | None
     format_template: str | None
+    discriminator: str | None
 
     def __init__(
         self,
         *,
         alias: str | None = None,
         format: PropertyFormat | None = None,
         format_template: str | None = None,
+        discriminator: str | None = None,
     ) -> None:
         self.alias = alias
         self.format = format
         self.format_template = format_template
+        self.discriminator = discriminator
 
     @override
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(alias='{self.alias}', format={self.format}, format_template='{self.format_template}')"
+        return f"{self.__class__.__name__}(alias='{self.alias}', format={self.format}, format_template='{self.format_template}', discriminator='{self.discriminator}')"
 
 
 def maybe_transform(
     data: object,
     expected_type: object,
 ) -> Any | None:
     """Wrapper over `transform()` that allows `None` to be passed.
```

### Comparing `groq-0.5.0/src/groq/_utils/_typing.py` & `groq-0.6.0/src/groq/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `groq-0.5.0/src/groq/_utils/_utils.py` & `groq-0.6.0/src/groq/_utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,16 @@
             else:  # no break
                 if len(variants) > 1:
                     variations = human_join(
                         ["(" + human_join([quote(arg) for arg in variant], final="and") + ")" for variant in variants]
                     )
                     msg = f"Missing required arguments; Expected either {variations} arguments to be given"
                 else:
+                    assert len(variants) > 0
+
                     # TODO: this error message is not deterministic
                     missing = list(set(variants[0]) - given_params)
                     if len(missing) > 1:
                         msg = f"Missing required arguments: {human_join([quote(arg) for arg in missing])}"
                     else:
                         msg = f"Missing required argument: {quote(missing[0])}"
                 raise TypeError(msg)
@@ -385,7 +387,17 @@
 
 
 def get_async_library() -> str:
     try:
         return sniffio.current_async_library()
     except Exception:
         return "false"
+
+
+def lru_cache(*, maxsize: int | None = 128) -> Callable[[CallableT], CallableT]:
+    """A version of functools.lru_cache that retains the type signature
+    for the wrapped function arguments.
+    """
+    wrapper = functools.lru_cache(  # noqa: TID251
+        maxsize=maxsize,
+    )
+    return cast(Any, wrapper)  # type: ignore[no-any-return]
```

### Comparing `groq-0.5.0/src/groq/lib/chat_completion_chunk.py` & `groq-0.6.0/src/groq/lib/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `groq-0.5.0/src/groq/resources/__init__.py` & `groq-0.6.0/src/groq/resources/chat/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,33 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from .chat import (
     Chat,
     AsyncChat,
     ChatWithRawResponse,
     AsyncChatWithRawResponse,
     ChatWithStreamingResponse,
     AsyncChatWithStreamingResponse,
 )
-from .audio import (
-    Audio,
-    AsyncAudio,
-    AudioWithRawResponse,
-    AsyncAudioWithRawResponse,
-    AudioWithStreamingResponse,
-    AsyncAudioWithStreamingResponse,
-)
-from .models import (
-    Models,
-    AsyncModels,
-    ModelsWithRawResponse,
-    AsyncModelsWithRawResponse,
-    ModelsWithStreamingResponse,
-    AsyncModelsWithStreamingResponse,
+from .completions import (
+    Completions,
+    AsyncCompletions,
+    CompletionsWithRawResponse,
+    AsyncCompletionsWithRawResponse,
+    CompletionsWithStreamingResponse,
+    AsyncCompletionsWithStreamingResponse,
 )
 
 __all__ = [
+    "Completions",
+    "AsyncCompletions",
+    "CompletionsWithRawResponse",
+    "AsyncCompletionsWithRawResponse",
+    "CompletionsWithStreamingResponse",
+    "AsyncCompletionsWithStreamingResponse",
     "Chat",
     "AsyncChat",
     "ChatWithRawResponse",
     "AsyncChatWithRawResponse",
     "ChatWithStreamingResponse",
     "AsyncChatWithStreamingResponse",
-    "Audio",
-    "AsyncAudio",
-    "AudioWithRawResponse",
-    "AsyncAudioWithRawResponse",
-    "AudioWithStreamingResponse",
-    "AsyncAudioWithStreamingResponse",
-    "Models",
-    "AsyncModels",
-    "ModelsWithRawResponse",
-    "AsyncModelsWithRawResponse",
-    "ModelsWithStreamingResponse",
-    "AsyncModelsWithStreamingResponse",
 ]
```

### Comparing `groq-0.5.0/src/groq/resources/models.py` & `groq-0.6.0/src/groq/resources/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 import httpx
 
-from ..types import Model, ModelList
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
 from .._compat import cached_property
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
+from ..types.model import Model
 from .._base_client import (
     make_request_options,
 )
+from ..types.model_list import ModelList
 
 __all__ = ["Models", "AsyncModels"]
 
 
 class Models(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> ModelsWithRawResponse:
```

### Comparing `groq-0.5.0/src/groq/resources/audio/__init__.py` & `groq-0.6.0/src/groq/resources/audio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from .audio import (
     Audio,
     AsyncAudio,
     AudioWithRawResponse,
     AsyncAudioWithRawResponse,
     AudioWithStreamingResponse,
```

### Comparing `groq-0.5.0/src/groq/resources/audio/audio.py` & `groq-0.6.0/src/groq/resources/audio/audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from .translations import (
     Translations,
```

### Comparing `groq-0.5.0/src/groq/resources/audio/transcriptions.py` & `groq-0.6.0/src/groq/resources/audio/transcriptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import List, Union, Mapping, cast
+from typing import Any, List, Union, Mapping, cast
 from typing_extensions import Literal
 
 import httpx
 
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven, FileTypes
 from ..._utils import (
     extract_files,
@@ -18,18 +18,19 @@
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
-from ...types.audio import Transcription, transcription_create_params
+from ...types.audio import transcription_create_params
 from ..._base_client import (
     make_request_options,
 )
+from ...types.audio.transcription_create_response import TranscriptionCreateResponse
 
 __all__ = ["Transcriptions", "AsyncTranscriptions"]
 
 
 class Transcriptions(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> TranscriptionsWithRawResponse:
@@ -51,15 +52,15 @@
         timestamp_granularities: List[Literal["word", "segment"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Transcription:
+    ) -> TranscriptionCreateResponse:
         """
         Transcribes audio into the input language.
 
         Args:
           file:
               The audio file object (not file name) to transcribe, in one of these formats:
               flac, mp3, mp4, mpeg, mpga, m4a, ogg, wav, or webm.
@@ -110,22 +111,27 @@
         )
         files = extract_files(cast(Mapping[str, object], body), paths=[["file"]])
         if files:
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
             extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
-        return self._post(
-            "/openai/v1/audio/transcriptions",
-            body=maybe_transform(body, transcription_create_params.TranscriptionCreateParams),
-            files=files,
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+        return cast(
+            TranscriptionCreateResponse,
+            self._post(
+                "/openai/v1/audio/transcriptions",
+                body=maybe_transform(body, transcription_create_params.TranscriptionCreateParams),
+                files=files,
+                options=make_request_options(
+                    extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                ),
+                cast_to=cast(
+                    Any, TranscriptionCreateResponse
+                ),  # Union types cannot be passed in as arguments in the type system
             ),
-            cast_to=Transcription,
         )
 
 
 class AsyncTranscriptions(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncTranscriptionsWithRawResponse:
         return AsyncTranscriptionsWithRawResponse(self)
@@ -146,15 +152,15 @@
         timestamp_granularities: List[Literal["word", "segment"]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Transcription:
+    ) -> TranscriptionCreateResponse:
         """
         Transcribes audio into the input language.
 
         Args:
           file:
               The audio file object (not file name) to transcribe, in one of these formats:
               flac, mp3, mp4, mpeg, mpga, m4a, ogg, wav, or webm.
@@ -205,22 +211,27 @@
         )
         files = extract_files(cast(Mapping[str, object], body), paths=[["file"]])
         if files:
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
             extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
-        return await self._post(
-            "/openai/v1/audio/transcriptions",
-            body=await async_maybe_transform(body, transcription_create_params.TranscriptionCreateParams),
-            files=files,
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+        return cast(
+            TranscriptionCreateResponse,
+            await self._post(
+                "/openai/v1/audio/transcriptions",
+                body=await async_maybe_transform(body, transcription_create_params.TranscriptionCreateParams),
+                files=files,
+                options=make_request_options(
+                    extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                ),
+                cast_to=cast(
+                    Any, TranscriptionCreateResponse
+                ),  # Union types cannot be passed in as arguments in the type system
             ),
-            cast_to=Transcription,
         )
 
 
 class TranscriptionsWithRawResponse:
     def __init__(self, transcriptions: Transcriptions) -> None:
         self._transcriptions = transcriptions
```

### Comparing `groq-0.5.0/src/groq/resources/audio/translations.py` & `groq-0.6.0/src/groq/resources/audio/translations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Union, Mapping, cast
+from typing import Any, Union, Mapping, cast
 from typing_extensions import Literal
 
 import httpx
 
-from ...types import Translation
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven, FileTypes
 from ..._utils import (
     extract_files,
     maybe_transform,
     deepcopy_minimal,
     async_maybe_transform,
 )
@@ -23,14 +22,15 @@
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from ...types.audio import translation_create_params
 from ..._base_client import (
     make_request_options,
 )
+from ...types.audio.translation_create_response import TranslationCreateResponse
 
 __all__ = ["Translations", "AsyncTranslations"]
 
 
 class Translations(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> TranslationsWithRawResponse:
@@ -50,15 +50,15 @@
         temperature: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Translation:
+    ) -> TranslationCreateResponse:
         """
         Translates audio into English.
 
         Args:
           file: The audio file object (not file name) translate, in one of these formats: flac,
               mp3, mp4, mpeg, mpga, m4a, ogg, wav, or webm.
 
@@ -96,22 +96,27 @@
         )
         files = extract_files(cast(Mapping[str, object], body), paths=[["file"]])
         if files:
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
             extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
-        return self._post(
-            "/openai/v1/audio/translations",
-            body=maybe_transform(body, translation_create_params.TranslationCreateParams),
-            files=files,
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+        return cast(
+            TranslationCreateResponse,
+            self._post(
+                "/openai/v1/audio/translations",
+                body=maybe_transform(body, translation_create_params.TranslationCreateParams),
+                files=files,
+                options=make_request_options(
+                    extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                ),
+                cast_to=cast(
+                    Any, TranslationCreateResponse
+                ),  # Union types cannot be passed in as arguments in the type system
             ),
-            cast_to=Translation,
         )
 
 
 class AsyncTranslations(AsyncAPIResource):
     @cached_property
     def with_raw_response(self) -> AsyncTranslationsWithRawResponse:
         return AsyncTranslationsWithRawResponse(self)
@@ -130,15 +135,15 @@
         temperature: float | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> Translation:
+    ) -> TranslationCreateResponse:
         """
         Translates audio into English.
 
         Args:
           file: The audio file object (not file name) translate, in one of these formats: flac,
               mp3, mp4, mpeg, mpga, m4a, ogg, wav, or webm.
 
@@ -176,22 +181,27 @@
         )
         files = extract_files(cast(Mapping[str, object], body), paths=[["file"]])
         if files:
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
             extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
-        return await self._post(
-            "/openai/v1/audio/translations",
-            body=await async_maybe_transform(body, translation_create_params.TranslationCreateParams),
-            files=files,
-            options=make_request_options(
-                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+        return cast(
+            TranslationCreateResponse,
+            await self._post(
+                "/openai/v1/audio/translations",
+                body=await async_maybe_transform(body, translation_create_params.TranslationCreateParams),
+                files=files,
+                options=make_request_options(
+                    extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+                ),
+                cast_to=cast(
+                    Any, TranslationCreateResponse
+                ),  # Union types cannot be passed in as arguments in the type system
             ),
-            cast_to=Translation,
         )
 
 
 class TranslationsWithRawResponse:
     def __init__(self, translations: Translations) -> None:
         self._translations = translations
```

### Comparing `groq-0.5.0/src/groq/resources/chat/chat.py` & `groq-0.6.0/src/groq/resources/chat/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from ..._compat import cached_property
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from .completions import (
     Completions,
```

### Comparing `groq-0.5.0/src/groq/resources/chat/completions.py` & `groq-0.6.0/src/groq/resources/chat/completions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Dict, List, Union, Iterable, Optional, overload
 from typing_extensions import Literal
 
 import httpx
@@ -17,19 +17,20 @@
 from ..._response import (
     to_raw_response_wrapper,
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from ..._streaming import Stream, AsyncStream
-from ...types.chat import ChatCompletion, completion_create_params
+from ...types.chat import completion_create_params
 from ..._base_client import (
     make_request_options,
 )
 from ...lib.chat_completion_chunk import ChatCompletionChunk
+from ...types.chat.chat_completion import ChatCompletion
 
 __all__ = ["Completions", "AsyncCompletions"]
 
 
 class Completions(SyncAPIResource):
     @cached_property
     def with_raw_response(self) -> CompletionsWithRawResponse:
```

### Comparing `groq-0.5.0/src/groq/types/audio/transcription_create_params.py` & `groq-0.6.0/src/groq/types/audio/transcription_create_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import List, Union
 from typing_extensions import Literal, Required, TypedDict
 
 from ..._types import FileTypes
```

### Comparing `groq-0.5.0/src/groq/types/audio/translation_create_params.py` & `groq-0.6.0/src/groq/types/audio/translation_create_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from typing import Union
 from typing_extensions import Literal, Required, TypedDict
 
 from ..._types import FileTypes
```

### Comparing `groq-0.5.0/src/groq/types/chat/chat_completion.py` & `groq-0.6.0/src/groq/types/chat/chat_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# File generated from our OpenAPI spec by Stainless.
+# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from typing import List, Optional
 
 from ..._models import BaseModel
 
 __all__ = [
     "ChatCompletion",
```

### Comparing `groq-0.5.0/LICENSE` & `groq-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `groq-0.5.0/README.md` & `groq-0.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,70 @@
+Metadata-Version: 2.3
+Name: groq
+Version: 0.6.0
+Summary: The official Python library for the groq API
+Project-URL: Homepage, https://github.com/groq/groq-python
+Project-URL: Repository, https://github.com/groq/groq-python
+Author-email: Groq <support@groq.com>
+License-Expression: Apache-2.0
+License-File: LICENSE
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Requires-Dist: anyio<5,>=3.5.0
+Requires-Dist: cached-property; python_version < '3.8'
+Requires-Dist: distro<2,>=1.7.0
+Requires-Dist: httpx<1,>=0.23.0
+Requires-Dist: pydantic<3,>=1.9.0
+Requires-Dist: sniffio
+Requires-Dist: typing-extensions<5,>=4.7
+Description-Content-Type: text/markdown
+
 # Groq Python API library
 
 [![PyPI version](https://img.shields.io/pypi/v/groq.svg)](https://pypi.org/project/groq/)
 
 The Groq Python library provides convenient access to the Groq REST API from any Python 3.7+
 application. The library includes type definitions for all request params and response fields,
 and offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).
 
+It is generated with [Stainless](https://www.stainlessapi.com/).
+
 ## Documentation
 
-The REST API documentation can be found [on console.groq.com](https://console.groq.com/docs). The full API of this library can be found in [api.md](api.md).
+The REST API documentation can be found [on console.groq.com](https://console.groq.com/docs). The full API of this library can be found in [api.md](https://github.com/groq/groq-python/tree/main/api.md).
 
 ## Installation
 
 ```sh
 # install from PyPI
 pip install groq
 ```
 
 ## Usage
 
-The full API of this library can be found in [api.md](api.md).
+The full API of this library can be found in [api.md](https://github.com/groq/groq-python/tree/main/api.md).
 
 ```python
-import os
 from groq import Groq
 
-client = Groq(
-    # This is the default and can be omitted
-    api_key=os.environ.get("GROQ_API_KEY"),
-)
+client = Groq()
 
 chat_completion = client.chat.completions.create(
     messages=[
         {
             "role": "user",
             "content": "Explain the importance of low latency LLMs",
         }
@@ -48,22 +80,18 @@
 so that your API Key is not stored in source control.
 
 ## Async usage
 
 Simply import `AsyncGroq` instead of `Groq` and use `await` with each API call:
 
 ```python
-import os
 import asyncio
 from groq import AsyncGroq
 
-client = AsyncGroq(
-    # This is the default and can be omitted
-    api_key=os.environ.get("GROQ_API_KEY"),
-)
+client = AsyncGroq()
 
 
 async def main() -> None:
     chat_completion = await client.chat.completions.create(
         messages=[
             {
                 "role": "user",
@@ -78,18 +106,18 @@
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
 ## Using types
 
-Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict). Responses are [Pydantic models](https://docs.pydantic.dev), which provide helper methods for things like:
+Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict). Responses are [Pydantic models](https://docs.pydantic.dev) which also provide helper methods for things like:
 
-- Serializing back into JSON, `model.model_dump_json(indent=2, exclude_unset=True)`
-- Converting to a dictionary, `model.model_dump(exclude_unset=True)`
+- Serializing back into JSON, `model.to_json()`
+- Converting to a dictionary, `model.to_dict()`
 
 Typed requests and responses provide autocomplete and documentation within your editor. If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `basic`.
 
 ## Handling errors
 
 When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `groq.APIConnectionError` is raised.
 
@@ -105,15 +133,15 @@
 client = Groq()
 
 try:
     client.chat.completions.create(
         messages=[
             {
                 "role": "system",
-                "content": "You are a helpful assisstant.",
+                "content": "You are a helpful assistant.",
             },
             {
                 "role": "user",
                 "content": "Explain the importance of low latency LLMs",
             },
         ],
         model="mixtral-8x7b-32768",
@@ -160,15 +188,15 @@
 )
 
 # Or, configure per-request:
 client.with_options(max_retries=5).chat.completions.create(
     messages=[
         {
             "role": "system",
-            "content": "You are a helpful assisstant.",
+            "content": "You are a helpful assistant.",
         },
         {
             "role": "user",
             "content": "Explain the importance of low latency LLMs",
         },
     ],
     model="mixtral-8x7b-32768",
@@ -191,32 +219,32 @@
 
 # More granular control:
 client = Groq(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-client.with_options(timeout=5 * 1000).chat.completions.create(
+client.with_options(timeout=5.0).chat.completions.create(
     messages=[
         {
             "role": "system",
-            "content": "You are a helpful assisstant.",
+            "content": "You are a helpful assistant.",
         },
         {
             "role": "user",
             "content": "Explain the importance of low latency LLMs",
         },
     ],
     model="mixtral-8x7b-32768",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
-Note that requests that time out are [retried twice by default](#retries).
+Note that requests that time out are [retried twice by default](https://github.com/groq/groq-python/tree/main/#retries).
 
 ## Advanced
 
 ### Logging
 
 We use the standard library [`logging`](https://docs.python.org/3/library/logging.html) module.
 
@@ -245,15 +273,15 @@
 ```py
 from groq import Groq
 
 client = Groq()
 response = client.chat.completions.with_raw_response.create(
     messages=[{
         "role": "system",
-        "content": "You are a helpful assisstant.",
+        "content": "You are a helpful assistant.",
     }, {
         "role": "user",
         "content": "Explain the importance of low latency LLMs",
     }],
     model="mixtral-8x7b-32768",
 )
 print(response.headers.get('X-My-Header'))
@@ -273,15 +301,15 @@
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
 with client.chat.completions.with_streaming_response.create(
     messages=[
         {
             "role": "system",
-            "content": "You are a helpful assisstant.",
+            "content": "You are a helpful assistant.",
         },
         {
             "role": "user",
             "content": "Explain the importance of low latency LLMs",
         },
     ],
     model="mixtral-8x7b-32768",
@@ -290,30 +318,64 @@
 
     for line in response.iter_lines():
         print(line)
 ```
 
 The context manager is required so that the response will reliably be closed.
 
+### Making custom/undocumented requests
+
+This library is typed for convenient access to the documented API.
+
+If you need to access undocumented endpoints, params, or response properties, the library can still be used.
+
+#### Undocumented endpoints
+
+To make requests to undocumented endpoints, you can make requests using `client.get`, `client.post`, and other
+http verbs. Options on the client will be respected (such as retries) will be respected when making this
+request.
+
+```py
+import httpx
+
+response = client.post(
+    "/foo",
+    cast_to=httpx.Response,
+    body={"my_param": True},
+)
+
+print(response.headers.get("x-foo"))
+```
+
+#### Undocumented request params
+
+If you want to explicitly send an extra param, you can do so with the `extra_query`, `extra_body`, and `extra_headers` request
+options.
+
+#### Undocumented response properties
+
+To access undocumented response properties, you can access the extra fields like `response.unknown_prop`. You
+can also get all the extra fields on the Pydantic model as a dict with
+[`response.model_extra`](https://docs.pydantic.dev/latest/api/base_model/#pydantic.BaseModel.model_extra).
+
 ### Configuring the HTTP client
 
 You can directly override the [httpx client](https://www.python-httpx.org/api/#client) to customize it for your use case, including:
 
 - Support for proxies
 - Custom transports
 - Additional [advanced](https://www.python-httpx.org/advanced/#client-instances) functionality
 
 ```python
-import httpx
-from groq import Groq
+from groq import Groq, DefaultHttpxClient
 
 client = Groq(
     # Or use the `GROQ_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
-    http_client=httpx.Client(
+    http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
     ),
 )
 ```
 
 ### Managing HTTP resources
```

