# Comparing `tmp/google_sheets_sdk-0.1.8.tar.gz` & `tmp/google_sheets_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_sheets_sdk-0.1.8.tar", max compression
+gzip compressed data, was "google_sheets_sdk-0.2.0.tar", max compression
```

## Comparing `google_sheets_sdk-0.1.8.tar` & `google_sheets_sdk-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.1.8/README.md
--rw-r--r--   0        0        0       48 2024-05-15 17:45:20.372660 google_sheets_sdk-0.1.8/google_sheets_sdk/__init__.py
--rw-r--r--   0        0        0     2329 2024-05-15 17:44:47.449101 google_sheets_sdk-0.1.8/google_sheets_sdk/client/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 17:30:15.109120 google_sheets_sdk-0.1.8/google_sheets_sdk/common/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 17:30:20.273045 google_sheets_sdk-0.1.8/google_sheets_sdk/common/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-15 17:22:49.403931 google_sheets_sdk-0.1.8/google_sheets_sdk/core/__init__.py
--rw-r--r--   0        0        0     2977 2024-05-15 17:38:38.566077 google_sheets_sdk-0.1.8/google_sheets_sdk/core/models.py
--rw-r--r--   0        0        0      407 2024-05-15 17:45:41.028385 google_sheets_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-10 05:20:37.756477 google_sheets_sdk-0.2.0/README.md
+-rw-r--r--   0        0        0       48 2024-05-15 17:45:20.372660 google_sheets_sdk-0.2.0/google_sheets_sdk/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-15 18:39:17.070002 google_sheets_sdk-0.2.0/google_sheets_sdk/client/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 17:30:15.109120 google_sheets_sdk-0.2.0/google_sheets_sdk/common/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-15 18:17:45.658511 google_sheets_sdk-0.2.0/google_sheets_sdk/core/__init__.py
+-rw-r--r--   0        0        0     2660 2024-05-15 18:40:21.349199 google_sheets_sdk-0.2.0/google_sheets_sdk/core/models.py
+-rw-r--r--   0        0        0      338 2024-05-15 18:31:50.751394 google_sheets_sdk-0.2.0/google_sheets_sdk/core/settings.py
+-rw-r--r--   0        0        0      407 2024-05-15 18:38:40.262459 google_sheets_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 google_sheets_sdk-0.2.0/PKG-INFO
```

### Comparing `google_sheets_sdk-0.1.8/google_sheets_sdk/client/__init__.py` & `google_sheets_sdk-0.2.0/google_sheets_sdk/client/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from dataclasses import InitVar, dataclass, field
+from dataclasses import dataclass, field
 from typing import ClassVar
 
 from httpx import AsyncClient, HTTPStatusError
 
-from google_sheets_sdk.core import models
+from google_sheets_sdk.core import Settings, models
 
 
 @dataclass
 class Client:
     _BASE_URL: ClassVar[str] = "https://sheets.googleapis.com/"
 
-    _http_client: AsyncClient
+    http_client: AsyncClient
+    settings: Settings = field(
+        default_factory=Settings,  # type: ignore
+    )
+
     _token: models.Token = field(
         init=False,
     )
-    settings: InitVar[models.Settings]
 
-    def __post_init__(
-        self,
-        settings: models.Settings,
-    ):
+    def __post_init__(self):
         self._token = models.Token(
-            email=settings.CLIENT_EMAIL,
+            email=self.settings.CLIENT_EMAIL,
             base_url=self._BASE_URL,
-            scope=settings.SCOPE.unicode_string(),
-            private_key=settings.PRIVATE_KEY.replace(r"\n", "\n"),
-            private_key_id=settings.PRIVATE_KEY_ID,
+            scope=self.settings.SCOPE.unicode_string(),
+            private_key=self.settings.PRIVATE_KEY.replace(r"\n", "\n"),
+            private_key_id=self.settings.PRIVATE_KEY_ID,
         )
 
     async def batch_clear_values(
         self,
         spreadsheet_id: models.SpreadsheetId,
         ranges: list[models.Range],
     ) -> None:
         try:
-            response = await self._http_client.post(
+            response = await self.http_client.post(
                 url=f"{self._BASE_URL}v4/spreadsheets/{spreadsheet_id}/values:batchClear",
                 json={
                     "ranges": ranges,
                 },
                 headers={
                     "Authorization": f"Bearer {self._token.encoded}",
                 },
@@ -49,15 +49,15 @@
 
     async def batch_update_values(
         self,
         spreadsheet_id: models.SpreadsheetId,
         sheets: list[models.Sheet],
     ) -> models.BatchUpdateValuesResponse:
         try:
-            response = await self._http_client.post(
+            response = await self.http_client.post(
                 url=f"{self._BASE_URL}v4/spreadsheets/{spreadsheet_id}/values:batchUpdate",
                 json={
                     "valueInputOption": "USER_ENTERED",
                     "data": [
                         sheet.model_dump(
                             mode="json",
                         )
```

### Comparing `google_sheets_sdk-0.1.8/google_sheets_sdk/core/models.py` & `google_sheets_sdk-0.2.0/google_sheets_sdk/core/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 import time as t
 from dataclasses import InitVar, dataclass, field
 
 from jose import jwt
 from pydantic import BaseModel
 from pydantic.fields import Field
-from pydantic.networks import EmailStr, HttpUrl
-from pydantic_settings import BaseSettings, SettingsConfigDict
 
 type Range = str
 type Value = str | int | float
 type SpreadsheetId = str
 
 
-class Settings(BaseSettings):
-    model_config = SettingsConfigDict(
-        env_prefix="GOOGLE_SHEETS_",
-    )
-
-    PRIVATE_KEY_ID: str
-    PRIVATE_KEY: str
-    CLIENT_EMAIL: EmailStr
-    SCOPE: HttpUrl
-
-
 class Sheet(BaseModel):
     range: Range
     values: list[list[Value]]
 
 
 @dataclass
 class Token:
```

### Comparing `google_sheets_sdk-0.1.8/PKG-INFO` & `google_sheets_sdk-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-sheets-sdk
-Version: 0.1.8
+Version: 0.2.0
 Summary: 
 Author: Marco Carmona
 Author-email: marcocarmonapy@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

