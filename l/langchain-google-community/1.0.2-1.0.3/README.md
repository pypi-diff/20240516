# Comparing `tmp/langchain_google_community-1.0.2.tar.gz` & `tmp/langchain_google_community-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_community-1.0.2.tar", max compression
+gzip compressed data, was "langchain_google_community-1.0.3.tar", max compression
```

## Comparing `langchain_google_community-1.0.2.tar` & `langchain_google_community-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1072 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/LICENSE
--rw-r--r--   0        0        0      258 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/README.md
--rw-r--r--   0        0        0     1964 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/__init__.py
--rw-r--r--   0        0        0     1262 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/_utils.py
--rw-r--r--   0        0        0     3712 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/bigquery.py
--rw-r--r--   0        0        0    34578 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/bigquery_vector_search.py
--rw-r--r--   0        0        0    15569 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/docai.py
--rw-r--r--   0        0        0     4620 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/documentai_warehouse.py
--rw-r--r--   0        0        0    17200 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/drive.py
--rw-r--r--   0        0        0     2123 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gcs_directory.py
--rw-r--r--   0        0        0     3549 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gcs_file.py
--rw-r--r--   0        0        0        0 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/__init__.py
--rw-r--r--   0        0        0     1029 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/base.py
--rw-r--r--   0        0        0     2565 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/create_draft.py
--rw-r--r--   0        0        0     2204 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/get_message.py
--rw-r--r--   0        0        0     1561 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/get_thread.py
--rw-r--r--   0        0        0     4062 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/loader.py
--rw-r--r--   0        0        0     5113 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/search.py
--rw-r--r--   0        0        0     2940 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/send_message.py
--rw-r--r--   0        0        0     2070 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/toolkit.py
--rw-r--r--   0        0        0     4624 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/utils.py
--rw-r--r--   0        0        0     5099 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/google_speech_to_text.py
--rw-r--r--   0        0        0     5071 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/places_api.py
--rw-r--r--   0        0        0     6413 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/search.py
--rw-r--r--   0        0        0     3217 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/texttospeech.py
--rw-r--r--   0        0        0     4188 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/translate.py
--rw-r--r--   0        0        0    19216 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/vertex_ai_search.py
--rw-r--r--   0        0        0     2975 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/vision.py
--rw-r--r--   0        0        0     2854 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 langchain_google_community-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/LICENSE
+-rw-r--r--   0        0        0      258 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/README.md
+-rw-r--r--   0        0        0     2048 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/__init__.py
+-rw-r--r--   0        0        0     1321 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/_utils.py
+-rw-r--r--   0        0        0     3765 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/bigquery.py
+-rw-r--r--   0        0        0    34651 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/bigquery_vector_search.py
+-rw-r--r--   0        0        0    15752 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/docai.py
+-rw-r--r--   0        0        0     4673 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/documentai_warehouse.py
+-rw-r--r--   0        0        0    22477 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/drive.py
+-rw-r--r--   0        0        0     2167 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gcs_directory.py
+-rw-r--r--   0        0        0     3599 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gcs_file.py
+-rw-r--r--   0        0        0        0 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gmail/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gmail/base.py
+-rw-r--r--   0        0        0     2565 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gmail/create_draft.py
+-rw-r--r--   0        0        0     2204 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gmail/get_message.py
+-rw-r--r--   0        0        0     1561 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gmail/get_thread.py
+-rw-r--r--   0        0        0     4062 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gmail/loader.py
+-rw-r--r--   0        0        0     5113 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gmail/search.py
+-rw-r--r--   0        0        0     2941 2024-04-26 16:51:47.911234 langchain_google_community-1.0.3/langchain_google_community/gmail/send_message.py
+-rw-r--r--   0        0        0     2070 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/gmail/toolkit.py
+-rw-r--r--   0        0        0     4650 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/gmail/utils.py
+-rw-r--r--   0        0        0     5201 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/google_speech_to_text.py
+-rw-r--r--   0        0        0     5130 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/places_api.py
+-rw-r--r--   0        0        0     6388 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/search.py
+-rw-r--r--   0        0        0     3296 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/texttospeech.py
+-rw-r--r--   0        0        0     4356 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/translate.py
+-rw-r--r--   0        0        0    19323 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/vertex_ai_search.py
+-rw-r--r--   0        0        0     6884 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/vertex_rank.py
+-rw-r--r--   0        0        0     3109 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/langchain_google_community/vision.py
+-rw-r--r--   0        0        0     4457 2024-04-26 16:51:47.915234 langchain_google_community-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2730 1970-01-01 00:00:00.000000 langchain_google_community-1.0.3/PKG-INFO
```

### Comparing `langchain_google_community-1.0.2/LICENSE` & `langchain_google_community-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.2/langchain_google_community/__init__.py` & `langchain_google_community-1.0.3/langchain_google_community/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from langchain_google_community.texttospeech import TextToSpeechTool
 from langchain_google_community.translate import GoogleTranslateTransformer
 from langchain_google_community.vertex_ai_search import (
     VertexAIMultiTurnSearchRetriever,
     VertexAISearchRetriever,
     VertexAISearchSummaryTool,
 )
+from langchain_google_community.vertex_rank import VertexAIRank
 from langchain_google_community.vision import CloudVisionLoader, CloudVisionParser
 
 __all__ = [
     "BigQueryLoader",
     "BigQueryVectorSearch",
     "CloudVisionLoader",
     "CloudVisionParser",
@@ -46,8 +47,9 @@
     "GoogleSearchRun",
     "GoogleTranslateTransformer",
     "SpeechToTextLoader",
     "TextToSpeechTool",
     "VertexAIMultiTurnSearchRetriever",
     "VertexAISearchRetriever",
     "VertexAISearchSummaryTool",
+    "VertexAIRank",
 ]
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/_utils.py` & `langchain_google_community-1.0.3/langchain_google_community/_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,21 +12,24 @@
     Args:
         module (Optional[str]):
             Optional. The module for a custom user agent header.
     Returns:
         Tuple[str, str]
     """
     try:
-        langchain_version = metadata.version("langchain")
+        langchain_version = metadata.version("langchain-google-community")
     except metadata.PackageNotFoundError:
         langchain_version = "0.0.0"
     client_library_version = (
         f"{langchain_version}-{module}" if module else langchain_version
     )
-    return client_library_version, f"langchain/{client_library_version}"
+    return (
+        client_library_version,
+        f"langchain-google-community/{client_library_version}",
+    )
 
 
 def get_client_info(module: Optional[str] = None) -> "ClientInfo":
     r"""Returns a client info object with a custom user agent header.
 
     Args:
         module (Optional[str]):
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/bigquery.py` & `langchain_google_community-1.0.3/langchain_google_community/bigquery.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,16 @@
 
     def load(self) -> List[Document]:
         try:
             from google.cloud import bigquery  # type: ignore[attr-defined]
         except ImportError as ex:
             raise ImportError(
                 "Could not import google-cloud-bigquery python package. "
-                "Please install it with `pip install google-cloud-bigquery`."
+                "Please, install bigquery dependency group: "
+                "`pip install langchain-google-community[bigquery]`"
             ) from ex
 
         bq_client = bigquery.Client(
             credentials=self.credentials,
             project=self.project,
             client_info=get_client_info(module="bigquery"),
         )
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/bigquery_vector_search.py` & `langchain_google_community-1.0.3/langchain_google_community/bigquery_vector_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Vector Store in Google Cloud BigQuery."""
+
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import sys
 import uuid
@@ -96,16 +97,17 @@
                 project=project_id,
                 location=location,
                 credentials=credentials,
                 client_info=client_info,
             )
         except ModuleNotFoundError:
             raise ImportError(
-                "Please, install or upgrade the google-cloud-bigquery library: "
-                "pip install google-cloud-bigquery"
+                "Could not import google-cloud-bigquery python package. "
+                "Please, install bigquery dependency group: "
+                "`pip install langchain-google-community[bigquery]`"
             )
         self._logger = logging.getLogger(__name__)
         self._creating_index = False
         self._have_index = False
         self.embedding_model = embedding
         self.project_id = project_id
         self.dataset_name = dataset_name
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/docai.py` & `langchain_google_community-1.0.3/langchain_google_community/docai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Module contains a PDF parser based on Document AI from Google Cloud.
 
 You need to install two libraries to use this parser:
 pip install google-cloud-documentai
 pip install google-cloud-documentai-toolbox
 """
+
 import logging
 import re
 import time
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Iterator, List, Optional, Sequence
 
 from langchain_core.document_loaders import BaseBlobParser
@@ -85,16 +86,17 @@
             self._client = client
         else:
             try:
                 from google.api_core.client_options import ClientOptions
                 from google.cloud.documentai import DocumentProcessorServiceClient
             except ImportError as exc:
                 raise ImportError(
-                    "documentai package not found, please install it with"
-                    " `pip install google-cloud-documentai`"
+                    "Could not import google-cloud-documentai python package. "
+                    "Please, install docai dependency group: "
+                    "`pip install langchain-google-community[docai]`"
                 ) from exc
             options = ClientOptions(
                 api_endpoint=f"{location}-documentai.googleapis.com"
             )
             self._client = DocumentProcessorServiceClient(
                 client_options=options,
                 client_info=get_client_info(module="document-ai"),
@@ -134,25 +136,26 @@
             from google.cloud.documentai_v1.types import (  # type: ignore[import, attr-defined]
                 IndividualPageSelector,
                 OcrConfig,
                 ProcessOptions,
             )
         except ImportError as exc:
             raise ImportError(
-                "documentai package not found, please install it with"
-                " `pip install google-cloud-documentai`"
+                "Could not import google-cloud-documentai python package. "
+                "Please, install docai dependency group: "
+                "`pip install langchain-google-community[docai]`"
             ) from exc
         try:
             from google.cloud.documentai_toolbox.wrappers.page import (  # type: ignore[import]
                 _text_from_layout,
             )
         except ImportError as exc:
             raise ImportError(
-                "documentai_toolbox package not found, please install it with"
-                " `pip install google-cloud-documentai-toolbox`"
+                "documentai_toolbox package not found, please install it with "
+                "`pip install langchain-google-community[docai]`"
             ) from exc
         ocr_config = (
             OcrConfig(enable_native_pdf_parsing=enable_native_pdf_parsing)
             if enable_native_pdf_parsing
             else None
         )
         individual_page_selector = (
@@ -243,16 +246,16 @@
             )
             from google.cloud.documentai_toolbox.wrappers.document import (  # type: ignore[import]
                 _get_shards,
             )
             from google.cloud.documentai_toolbox.wrappers.page import _text_from_layout
         except ImportError as exc:
             raise ImportError(
-                "documentai_toolbox package not found, please install it with"
-                " `pip install google-cloud-documentai-toolbox`"
+                "documentai_toolbox package not found, please install it with "
+                "`pip install langchain-google-community[docai]`"
             ) from exc
         for result in results:
             gcs_bucket_name, gcs_prefix = split_gcs_uri(result.parsed_path)
             shards = _get_shards(gcs_bucket_name, gcs_prefix)
             yield from (
                 Document(
                     page_content=_text_from_layout(page.layout, shard.text),
@@ -267,15 +270,15 @@
         try:
             from google.longrunning.operations_pb2 import (  # type: ignore[import]
                 GetOperationRequest,
             )
         except ImportError as exc:
             raise ImportError(
                 "long running operations package not found, please install it with"
-                " `pip install gapic-google-longrunning`"
+                "`pip install langchain-google-community[docai]`"
             ) from exc
 
         return [
             self._client.get_operation(request=GetOperationRequest(name=name))
             for name in operation_names
         ]
 
@@ -310,16 +313,16 @@
         and results are stored in a output GCS bucket.
         """
         try:
             from google.cloud import documentai
             from google.cloud.documentai_v1.types import OcrConfig, ProcessOptions
         except ImportError as exc:
             raise ImportError(
-                "documentai package not found, please install it with"
-                " `pip install google-cloud-documentai`"
+                "documentai package not found, please install it with "
+                "`pip install langchain-google-community[docai]`"
             ) from exc
 
         output_path = gcs_output_path or self._gcs_output_path
         if output_path is None:
             raise ValueError(
                 "An output path on Google Cloud Storage should be provided."
             )
@@ -372,16 +375,16 @@
     def get_results(self, operations: List["Operation"]) -> List[DocAIParsingResults]:
         try:
             from google.cloud.documentai_v1 import (  # type: ignore[import]
                 BatchProcessMetadata,
             )
         except ImportError as exc:
             raise ImportError(
-                "documentai package not found, please install it with"
-                " `pip install google-cloud-documentai`"
+                "documentai package not found, please install it with "
+                "`pip install langchain-google-community[docai]`"
             ) from exc
 
         return [
             DocAIParsingResults(
                 source_path=status.input_gcs_source,
                 parsed_path=status.output_gcs_destination,
             )
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/documentai_warehouse.py` & `langchain_google_community-1.0.3/langchain_google_community/documentai_warehouse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Retriever wrapper for Google Cloud Document AI Warehouse."""
+
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from langchain_core.callbacks import CallbackManagerForRetrieverRun
 from langchain_core.documents import Document
 from langchain_core.pydantic_v1 import root_validator
 from langchain_core.retrievers import BaseRetriever
 from langchain_core.utils import get_from_dict_or_env
@@ -44,16 +45,17 @@
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validates the environment."""
         try:  # noqa: F401
             from google.cloud.contentwarehouse_v1 import DocumentServiceClient
         except ImportError as exc:
             raise ImportError(
-                "google.cloud.contentwarehouse is not installed."
-                "Please install it with pip install google-cloud-contentwarehouse"
+                "Could not import google-cloud-documentai python package. "
+                "Please, install docai dependency group: "
+                "`pip install langchain-google-community[docai]`"
             ) from exc
 
         values["project_number"] = get_from_dict_or_env(
             values, "project_number", "PROJECT_NUMBER"
         )
         values["client"] = DocumentServiceClient(
             client_info=get_client_info(module="document-ai-warehouse")
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/drive.py` & `langchain_google_community-1.0.3/langchain_google_community/drive.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,14 +43,116 @@
     # results in pydantic validation errors
     file_loader_cls: Any = None
     """The file loader class to use."""
     file_loader_kwargs: Dict["str", Any] = {}
     """The file loader kwargs to use."""
     load_auth: bool = False
     """Whether to load authorization identities."""
+    load_extended_metadata: bool = False
+    """Whether to load extended metadata."""
+
+    def _get_file_size_from_id(self, id: str) -> str:
+        """Fetch the size of the file."""
+        try:
+            import googleapiclient.errors  # type: ignore[import]
+            from googleapiclient.discovery import build  # type: ignore[import]
+        except ImportError as exc:
+            raise ImportError(
+                "You must run "
+                "`pip install --upgrade "
+                "google-api-python-client` "
+                "to load authorization identities."
+            ) from exc
+
+        creds = self._load_credentials()
+        service = build("drive", "v3", credentials=creds)
+        try:
+            file = service.files().get(fileId=id, fields="size").execute()
+            return file["size"]
+        except googleapiclient.errors.HttpError:
+            print(
+                f"insufficientFilePermissions: The user does not have sufficient \
+                permissions to retrieve size for the file with fileId: {id}"
+            )
+            return "unknown"
+        except Exception as exc:
+            print(
+                f"Error occurred while fetching the size for the file with fileId: {id}"
+            )
+            print(f"Error: {exc}")
+            return "unknown"
+
+    def _get_owner_metadata_from_id(self, id: str) -> str:
+        """Fetch the owner of the file."""
+        try:
+            import googleapiclient.errors  # type: ignore[import]
+            from googleapiclient.discovery import build  # type: ignore[import]
+        except ImportError as exc:
+            raise ImportError(
+                "You must run "
+                "`pip install --upgrade "
+                "google-api-python-client` "
+                "to load authorization identities."
+            ) from exc
+
+        creds = self._load_credentials()
+        service = build("drive", "v3", credentials=creds)
+        try:
+            file = service.files().get(fileId=id, fields="owners").execute()
+            return file["owners"][0].get("emailAddress")
+        except googleapiclient.errors.HttpError:
+            print(
+                f"insufficientFilePermissions: The user does not have sufficient \
+                permissions to retrieve owner for the file with fileId: {id}"
+            )
+            return "unknown"
+        except Exception as exc:
+            print(
+                f"Error occurred while fetching the owner for the file with fileId: \
+                {id} with error: {exc}"
+            )
+            return "unknown"
+
+    def _get_file_path_from_id(self, id: str) -> str:
+        """Fetch the full path of the file starting from the root."""
+        try:
+            import googleapiclient.errors  # type: ignore[import]
+            from googleapiclient.discovery import build  # type: ignore[import]
+        except ImportError as exc:
+            raise ImportError(
+                "You must run "
+                "`pip install --upgrade "
+                "google-api-python-client` "
+                "to load authorization identities."
+            ) from exc
+
+        creds = self._load_credentials()
+        service = build("drive", "v3", credentials=creds)
+        path = []
+        current_id = id
+        while True:
+            try:
+                file = (
+                    service.files()
+                    .get(fileId=current_id, fields="name, parents")
+                    .execute()
+                )
+                path.append(file["name"])
+                if "parents" in file:
+                    current_id = file["parents"][0]
+                else:
+                    break
+            except googleapiclient.errors.HttpError:
+                print(
+                    f"insufficientFilePermissions: The user does not have sufficient\
+                    permissions to retrieve path for the file with fileId: {id}"
+                )
+                break
+        path.reverse()
+        return "/".join(path)
 
     def _get_identity_metadata_from_id(self, id: str) -> List[str]:
         """Fetch the list of people having access to ID file."""
         try:
             import googleapiclient.errors  # type: ignore[import]
             from googleapiclient.discovery import build  # type: ignore[import]
         except ImportError as exc:
@@ -155,19 +257,17 @@
             from google.oauth2 import service_account  # type: ignore[import]
             from google.oauth2.credentials import Credentials  # type: ignore[import]
             from google_auth_oauthlib.flow import (  # type: ignore[import]
                 InstalledAppFlow,
             )
         except ImportError:
             raise ImportError(
-                "Install prerequisites by running: "
-                "`pip install --upgrade "
-                "google-api-python-client google-auth-httplib2 "
-                "google-auth-oauthlib` "
-                "to use the Google Drive loader."
+                "Could execute GoogleDriveLoader. "
+                "Please, install drive dependency group: "
+                "`pip install langchain-google-community[drive]`"
             )
 
         creds = None
         if self.service_account_key.exists():
             return service_account.Credentials.from_service_account_file(
                 str(self.service_account_key), scopes=SCOPES
             )
@@ -201,14 +301,18 @@
 
         creds = self._load_credentials()
         sheets_service = build("sheets", "v4", credentials=creds)
         spreadsheet = sheets_service.spreadsheets().get(spreadsheetId=id).execute()
         sheets = spreadsheet.get("sheets", [])
         if self.load_auth:
             authorized_identities = self._get_identity_metadata_from_id(id)
+        if self.load_extended_metadata:
+            owner = self._get_owner_metadata_from_id(id)
+            size = self._get_file_size_from_id(id)
+            full_path = self._get_file_path_from_id(id)
 
         documents = []
         for sheet in sheets:
             sheet_name = sheet["properties"]["title"]
             result = (
                 sheets_service.spreadsheets()
                 .values()
@@ -227,14 +331,18 @@
                         f"edit?gid={sheet['properties']['sheetId']}"
                     ),
                     "title": f"{spreadsheet['properties']['title']} - {sheet_name}",
                     "row": i,
                 }
                 if self.load_auth:
                     metadata["authorized_identities"] = authorized_identities
+                if self.load_extended_metadata:
+                    metadata["owner"] = owner
+                    metadata["size"] = size
+                    metadata["full_path"] = full_path
                 content = []
                 for j, v in enumerate(row):
                     title = header[j].strip() if len(header) > j else ""
                     content.append(f"{title}: {v.strip()}")
 
                 page_content = "\n".join(content)
                 documents.append(Document(page_content=page_content, metadata=metadata))
@@ -249,14 +357,18 @@
         from googleapiclient.errors import HttpError  # type: ignore[import]
         from googleapiclient.http import MediaIoBaseDownload  # type: ignore[import]
 
         creds = self._load_credentials()
         service = build("drive", "v3", credentials=creds)
         if self.load_auth:
             authorized_identities = self._get_identity_metadata_from_id(id)
+        if self.load_extended_metadata:
+            owner = self._get_owner_metadata_from_id(id)
+            size = self._get_file_size_from_id(id)
+            full_path = self._get_file_path_from_id(id)
 
         file = (
             service.files()
             .get(fileId=id, supportsAllDrives=True, fields="modifiedTime,name")
             .execute()
         )
         request = service.files().export_media(fileId=id, mimeType="text/plain")
@@ -277,14 +389,18 @@
         metadata = {
             "source": f"https://docs.google.com/document/d/{id}/edit",
             "title": f"{file.get('name')}",
             "when": f"{file.get('modifiedTime')}",
         }
         if self.load_auth:
             metadata["authorized_identities"] = authorized_identities  # type: ignore
+        if self.load_extended_metadata:
+            metadata["owner"] = owner
+            metadata["size"] = size
+            metadata["full_path"] = full_path
         return Document(page_content=text, metadata=metadata)
 
     def _load_documents_from_folder(
         self, folder_id: str, *, file_types: Optional[Sequence[str]] = None
     ) -> List[Document]:
         """Load documents from a folder."""
         from googleapiclient.discovery import build
@@ -356,14 +472,18 @@
         from googleapiclient.http import MediaIoBaseDownload
 
         creds = self._load_credentials()
         service = build("drive", "v3", credentials=creds)
 
         if self.load_auth:
             authorized_identities = self._get_identity_metadata_from_id(id)
+        if self.load_extended_metadata:
+            owner = self._get_owner_metadata_from_id(id)
+            size = self._get_file_size_from_id(id)
+            full_path = self._get_file_path_from_id(id)
 
         file = service.files().get(fileId=id, supportsAllDrives=True).execute()
         request = service.files().get_media(fileId=id)
         fh = BytesIO()
         downloader = MediaIoBaseDownload(fh, request)
         done = False
         while done is False:
@@ -375,14 +495,18 @@
             docs = loader.load()
             for doc in docs:
                 doc.metadata["source"] = f"https://drive.google.com/file/d/{id}/view"
                 if "title" not in doc.metadata:
                     doc.metadata["title"] = f"{file.get('name')}"
                 if self.load_auth:
                     doc.metadata["authorized_identities"] = authorized_identities
+                if self.load_extended_metadata:
+                    doc.metadata["owner"] = owner
+                    doc.metadata["size"] = size
+                    doc.metadata["full_path"] = full_path
             return docs
 
         else:
             from PyPDF2 import PdfReader  # type: ignore[import]
 
             content = fh.getvalue()
             pdf_reader = PdfReader(BytesIO(content))
@@ -392,14 +516,18 @@
                 metadata = {
                     "source": f"https://drive.google.com/file/d/{id}/view",
                     "title": f"{file.get('name')}",
                     "page": i,
                 }
                 if self.load_auth:
                     metadata["authorized_identities"] = authorized_identities
+                if self.load_extended_metadata:
+                    metadata["owner"] = owner
+                    metadata["size"] = size
+                    metadata["full_path"] = full_path
                 docs.append(
                     Document(
                         page_content=page.extract_text(),
                         metadata=metadata,
                     )
                 )
             return docs
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gcs_directory.py` & `langchain_google_community-1.0.3/langchain_google_community/gcs_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     def load(self) -> List[Document]:
         """Load documents."""
         try:
             from google.cloud import storage  # type: ignore[attr-defined]
         except ImportError:
             raise ImportError(
                 "Could not import google-cloud-storage python package. "
-                "Please install it with `pip install google-cloud-storage`."
+                "Please, install gcs dependency group: "
+                "`pip install langchain-google-community[gcs]`"
             )
         client = storage.Client(
             project=self.project_name,
             client_info=get_client_info(module="google-cloud-storage"),
         )
         docs = []
         for blob in client.list_blobs(self.bucket, prefix=self.prefix):
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gcs_file.py` & `langchain_google_community-1.0.3/langchain_google_community/gcs_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,29 +47,30 @@
                 from langchain_community.document_loaders.unstructured import (
                     UnstructuredFileLoader,
                 )
             except ImportError:
                 message = (
                     "UnstructuredFileLoader loader not found! Either provide a "
                     "custom loader with loader_func argument, or install "
-                    " `pip install langchain_community`"
+                    "`pip install langchain-google-community`"
                 )
                 print(message)
             return UnstructuredFileLoader(file_path)
 
         self._loader_func = loader_func if loader_func else default_loader_func
 
     def load(self) -> List[Document]:
         """Load documents."""
         try:
             from google.cloud import storage  # type: ignore[attr-defined]
         except ImportError:
             raise ImportError(
                 "Could not import google-cloud-storage python package. "
-                "Please install it with `pip install google-cloud-storage`."
+                "Please, install gcs dependency group: "
+                "`pip install langchain-google-community[gcs]`"
             )
 
         # initialize a client
         storage_client = storage.Client(
             self.project_name, client_info=get_client_info("google-cloud-storage")
         )
         # Create a bucket object for our bucket
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gmail/base.py` & `langchain_google_community-1.0.3/langchain_google_community/gmail/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base class for Gmail tools."""
+
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from langchain_core.pydantic_v1 import Field
 from langchain_core.tools import BaseTool
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gmail/create_draft.py` & `langchain_google_community-1.0.3/langchain_google_community/gmail/create_draft.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gmail/get_message.py` & `langchain_google_community-1.0.3/langchain_google_community/gmail/get_message.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gmail/get_thread.py` & `langchain_google_community-1.0.3/langchain_google_community/gmail/get_thread.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gmail/loader.py` & `langchain_google_community-1.0.3/langchain_google_community/gmail/loader.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gmail/search.py` & `langchain_google_community-1.0.3/langchain_google_community/gmail/search.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gmail/send_message.py` & `langchain_google_community-1.0.3/langchain_google_community/gmail/send_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Send Gmail messages."""
+
 import base64
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from typing import Any, Dict, List, Optional, Type, Union
 
 from langchain_core.callbacks import CallbackManagerForToolRun
 from langchain_core.pydantic_v1 import BaseModel, Field
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gmail/toolkit.py` & `langchain_google_community-1.0.3/langchain_google_community/gmail/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.2/langchain_google_community/gmail/utils.py` & `langchain_google_community-1.0.3/langchain_google_community/gmail/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Gmail tool utils."""
+
 from __future__ import annotations
 
 import logging
 import os
 from typing import TYPE_CHECKING, List, Optional, Tuple
 
 if TYPE_CHECKING:
@@ -23,48 +24,49 @@
     """
     # google-auth-httplib2
     try:
         from google.auth.transport.requests import Request  # noqa: F401
         from google.oauth2.credentials import Credentials  # noqa: F401
     except ImportError:
         raise ImportError(
-            "You need to install google-auth-httplib2 to use this toolkit. "
-            "Try running pip install --upgrade google-auth-httplib2"
+            "You need to install gmail dependencies to use this toolkit. "
+            "Try running poetry install --with gmail"
         )
     return Request, Credentials
 
 
 def import_installed_app_flow() -> InstalledAppFlow:
     """Import InstalledAppFlow class.
 
     Returns:
         InstalledAppFlow: InstalledAppFlow class.
     """
     try:
         from google_auth_oauthlib.flow import InstalledAppFlow
     except ImportError:
         raise ImportError(
-            "You need to install google-auth-oauthlib to use this toolkit. "
-            "Try running pip install --upgrade google-auth-oauthlib"
+            "You need to install gmail dependencies to use this toolkit. "
+            "Please, install bigquery dependency group: "
+            "`pip install langchain-google-community[gmail]`"
         )
     return InstalledAppFlow
 
 
 def import_googleapiclient_resource_builder() -> build_resource:
     """Import googleapiclient.discovery.build function.
 
     Returns:
         build_resource: googleapiclient.discovery.build function.
     """
     try:
         from googleapiclient.discovery import build
     except ImportError:
         raise ImportError(
-            "You need to install googleapiclient to use this toolkit. "
-            "Try running pip install --upgrade google-api-python-client"
+            "You need to install all dependencies to use this toolkit. "
+            "Try running pip install langchain-google-community"
         )
     return build
 
 
 DEFAULT_SCOPES = ["https://mail.google.com/"]
 DEFAULT_CREDS_TOKEN_FILE = "token.json"
 DEFAULT_CLIENT_SECRETS_FILE = "credentials.json"
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/google_speech_to_text.py` & `langchain_google_community-1.0.3/langchain_google_community/google_speech_to_text.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,15 +62,16 @@
                 RecognitionConfig,
                 RecognitionFeatures,
                 SpeechClient,
             )
         except ImportError as exc:
             raise ImportError(
                 "Could not import google-cloud-speech python package. "
-                "Please install it with `pip install google-cloud-speech`."
+                "Please, install speech dependency group: "
+                "`pip install langchain-google-community[speech]`"
             ) from exc
 
         self.project_id = project_id
         self.file_path = file_path
         self.location = location
         self.recognizer_id = recognizer_id
         # Config must be set in speech recognition request.
@@ -104,15 +105,16 @@
         and blocks until the transcription is finished.
         """
         try:
             from google.cloud.speech_v2 import RecognizeRequest
         except ImportError as exc:
             raise ImportError(
                 "Could not import google-cloud-speech python package. "
-                "Please install it with `pip install google-cloud-speech`."
+                "Please, install speech dependency group: "
+                "`pip install langchain-google-community[speech]`"
             ) from exc
 
         request = RecognizeRequest(
             recognizer=self._recognizer_path,
             config=self.config,
             config_mask=self.config_mask,
         )
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/places_api.py` & `langchain_google_community-1.0.3/langchain_google_community/places_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Chain that calls Google Places API.
-"""
+"""Chain that calls Google Places API."""
 
 import logging
 from typing import Any, Dict, Optional, Type
 
 from langchain_core.callbacks import CallbackManagerForToolRun
 from langchain_core.pydantic_v1 import BaseModel, Extra, Field, root_validator
 from langchain_core.tools import BaseTool
@@ -50,15 +49,16 @@
         try:
             import googlemaps  # type: ignore[import]
 
             values["google_map_client"] = googlemaps.Client(gplaces_api_key)
         except ImportError:
             raise ImportError(
                 "Could not import googlemaps python package. "
-                "Please install it with `pip install googlemaps`."
+                "Please, install places dependency group: "
+                "`pip install langchain-google-community[places]`"
             )
         return values
 
     def run(self, query: str) -> str:
         """Run Places search and get k number of places that exists that match."""
         search_results = self.google_map_client.places(query)["results"]
         num_to_return = len(search_results)
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/search.py` & `langchain_google_community-1.0.3/langchain_google_community/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Util that calls Google Search."""
+
 from typing import Any, Dict, List, Optional
 
 from langchain_core.callbacks import CallbackManagerForToolRun
 from langchain_core.pydantic_v1 import BaseModel, Extra, root_validator
 from langchain_core.tools import BaseTool
 from langchain_core.utils import get_from_dict_or_env
 
@@ -77,16 +78,15 @@
 
         try:
             from googleapiclient.discovery import build  # type: ignore[import]
 
         except ImportError:
             raise ImportError(
                 "google-api-python-client is not installed. "
-                "Please install it with `pip install google-api-python-client"
-                ">=2.100.0`"
+                "Please install it with `pip install langchain-google-community`"
             )
 
         service = build("customsearch", "v1", developerKey=google_api_key)
         values["search_engine"] = service
 
         return values
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/texttospeech.py` & `langchain_google_community-1.0.3/langchain_google_community/texttospeech.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
 
 def _import_google_cloud_texttospeech() -> Any:
     try:
         from google.cloud import texttospeech  # type: ignore[attr-defined]
     except ImportError as e:
         raise ImportError(
-            "Cannot import google.cloud.texttospeech, please install "
-            "`pip install google-cloud-texttospeech`."
+            "Could not import google-cloud-texttospeech python package. "
+            "Please, install texttospeech dependency group: "
+            "`pip install langchain-google-community[texttospeech]`"
         ) from e
     return texttospeech
 
 
 def _encoding_file_extension_map(encoding: texttospeech.AudioEncoding) -> Optional[str]:
     texttospeech = _import_google_cloud_texttospeech()
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/translate.py` & `langchain_google_community-1.0.3/langchain_google_community/translate.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,17 @@
             api_endpoint: (Optional) Regional endpoint to use.
         """
         try:
             from google.api_core.client_options import ClientOptions
             from google.cloud import translate  # type: ignore[attr-defined]
         except ImportError as exc:
             raise ImportError(
-                "Install Google Cloud Translate to use this parser."
-                "(pip install google-cloud-translate)"
+                "Could not import google-cloud-translate python package. "
+                "Please, install translate dependency group: "
+                "`pip install langchain-google-community[translate]`"
             ) from exc
 
         self.project_id = project_id
         self.location = location
         self.model_id = model_id
         self.glossary_id = glossary_id
 
@@ -69,16 +70,17 @@
             mime_type: (Optional) Media Type of input text.
                 Options: `text/plain`, `text/html`
         """
         try:
             from google.cloud import translate  # type: ignore[attr-defined]
         except ImportError as exc:
             raise ImportError(
-                "Install Google Cloud Translate to use this parser."
-                "(pip install google-cloud-translate)"
+                "Could not import google-cloud-translate python package. "
+                "Please, install translate dependency group: "
+                "`pip install langchain-google-community[translate]`"
             ) from exc
 
         response = self._client.translate_text(
             request=translate.TranslateTextRequest(
                 contents=[doc.page_content for doc in documents],
                 parent=self._parent_path,
                 model=self._model_path,
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/vertex_ai_search.py` & `langchain_google_community-1.0.3/langchain_google_community/vertex_ai_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,17 +55,17 @@
     @root_validator(pre=True)
     def validate_environment(cls, values: Dict) -> Dict:
         """Validates the environment."""
         try:
             from google.cloud import discoveryengine_v1beta  # noqa: F401
         except ImportError as exc:
             raise ImportError(
-                "google.cloud.discoveryengine is not installed."
-                "Please install it with pip install "
-                "google-cloud-discoveryengine>=0.11.0"
+                "Could not import google-cloud-discoveryengine python package. "
+                "Please, install vertexaisearch dependency group: "
+                "poetry install --with vertexaisearch"
             ) from exc
 
         values["project_id"] = get_from_dict_or_env(values, "project_id", "PROJECT_ID")
 
         try:
             # For backwards compatibility
             search_engine_id = get_from_dict_or_env(
@@ -246,16 +246,17 @@
 
     def __init__(self, **kwargs: Any) -> None:
         """Initializes private fields."""
         try:
             from google.cloud.discoveryengine_v1beta import SearchServiceClient
         except ImportError as exc:
             raise ImportError(
-                "google.cloud.discoveryengine is not installed."
-                "Please install it with pip install google-cloud-discoveryengine"
+                "Could not import google-cloud-discoveryengine python package. "
+                "Please, install vertexaisearch dependency group: "
+                "`pip install langchain-google-community[vertexaisearch]`"
             ) from exc
 
         super().__init__(**kwargs)
 
         #  For more information, refer to:
         # https://cloud.google.com/generative-ai-app-builder/docs/locations#specify_a_multi-region_for_your_data_store
         self._client = SearchServiceClient(
```

### Comparing `langchain_google_community-1.0.2/langchain_google_community/vision.py` & `langchain_google_community-1.0.3/langchain_google_community/vision.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 class CloudVisionParser(BaseBlobParser):
     def __init__(self, project: Optional[str] = None):
         try:
             from google.cloud import vision  # type: ignore[attr-defined]
         except ImportError as e:
             raise ImportError(
-                "Cannot import google.cloud.vision, please install "
-                "`pip install google-cloud-vision`."
+                "Could not import google-cloud-vision python package. "
+                "Please, install vision dependency group: "
+                "poetry install --with vision"
             ) from e
         client_options = None
         if project:
             client_options = {"quota_project_id": project}
         self._client = vision.ImageAnnotatorClient(
             client_options=client_options,
             client_info=get_client_info(module="cloud-vision"),
@@ -44,16 +45,17 @@
 
 class CloudVisionLoader(BaseLoader):
     def __init__(self, file_path: str, project: Optional[str] = None):
         try:
             from google.cloud import vision  # type: ignore[attr-defined]
         except ImportError as e:
             raise ImportError(
-                "Cannot import google.cloud.vision, please install "
-                "`pip install google-cloud-vision`."
+                "Could not import google-cloud-vision python package. "
+                "Please, install vision dependency group: "
+                "`pip install langchain-google-community[vision]`"
             ) from e
         client_options = None
         if project:
             client_options = {"quota_project_id": project}
         self._client = vision.ImageAnnotatorClient(
             client_options=client_options,
             client_info=get_client_info(module="cloud-vision"),
```

