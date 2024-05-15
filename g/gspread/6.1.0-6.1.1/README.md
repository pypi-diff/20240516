# Comparing `tmp/gspread-6.1.0.tar.gz` & `tmp/gspread-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspread-6.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gspread-6.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gspread-6.1.0.tar` & `gspread-6.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    38380 2024-03-28 15:07:43.862427 gspread-6.1.0/HISTORY.rst
--rw-r--r--   0        0        0     1064 2024-03-28 15:07:43.862427 gspread-6.1.0/LICENSE.txt
--rw-r--r--   0        0        0     9272 2024-03-28 15:07:43.862427 gspread-6.1.0/README.md
--rw-r--r--   0        0        0     1301 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/_templates/layout.html
--rw-r--r--   0        0        0     2310 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/advanced.rst
--rw-r--r--   0        0        0       53 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/auth.rst
--rw-r--r--   0        0        0       58 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/client.rst
--rw-r--r--   0        0        0      472 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/exceptions.rst
--rw-r--r--   0        0        0      258 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/http_client.rst
--rw-r--r--   0        0        0      144 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/index.rst
--rw-r--r--   0        0        0       57 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/models/cell.rst
--rw-r--r--   0        0        0      432 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/models/index.rst
--rw-r--r--   0        0        0       85 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/models/spreadsheet.rst
--rw-r--r--   0        0        0      179 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/models/worksheet.rst
--rw-r--r--   0        0        0      128 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/top-level.rst
--rw-r--r--   0        0        0       75 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/api/utils.rst
--rw-r--r--   0        0        0     9539 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/conf.py
--rw-r--r--   0        0        0     2300 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/index.rst
--rw-r--r--   0        0        0    11204 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/oauth2.rst
--rw-r--r--   0        0        0       46 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/requirements.txt
--rw-r--r--   0        0        0    10345 2024-03-28 15:07:43.862427 gspread-6.1.0/docs/user-guide.rst
--rw-r--r--   0        0        0      560 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/__init__.py
--rw-r--r--   0        0        0    13963 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/auth.py
--rw-r--r--   0        0        0     2407 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/cell.py
--rw-r--r--   0        0        0    15606 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/client.py
--rw-r--r--   0        0        0     1713 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/exceptions.py
--rw-r--r--   0        0        0    22625 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/http_client.py
--rw-r--r--   0        0        0        0 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/py.typed
--rw-r--r--   0        0        0    27596 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/spreadsheet.py
--rw-r--r--   0        0        0     1287 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/urls.py
--rw-r--r--   0        0        0    26705 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/utils.py
--rw-r--r--   0        0        0   115449 2024-03-28 15:07:43.862427 gspread-6.1.0/gspread/worksheet.py
--rw-r--r--   0        0        0     1546 2024-03-28 15:07:43.862427 gspread-6.1.0/pyproject.toml
--rw-r--r--   0        0        0    10596 1970-01-01 00:00:00.000000 gspread-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0    39852 2024-05-15 23:22:07.109393 gspread-6.1.1/HISTORY.rst
+-rw-r--r--   0        0        0     1064 2024-05-15 23:22:07.109393 gspread-6.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     9779 2024-05-15 23:22:07.109393 gspread-6.1.1/README.md
+-rw-r--r--   0        0        0     1301 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/_templates/layout.html
+-rw-r--r--   0        0        0     2310 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/advanced.rst
+-rw-r--r--   0        0        0       53 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/auth.rst
+-rw-r--r--   0        0        0       58 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/client.rst
+-rw-r--r--   0        0        0      472 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/exceptions.rst
+-rw-r--r--   0        0        0      258 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/http_client.rst
+-rw-r--r--   0        0        0      144 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/index.rst
+-rw-r--r--   0        0        0       57 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/models/cell.rst
+-rw-r--r--   0        0        0      432 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/models/index.rst
+-rw-r--r--   0        0        0       85 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/models/spreadsheet.rst
+-rw-r--r--   0        0        0      179 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/models/worksheet.rst
+-rw-r--r--   0        0        0      128 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/top-level.rst
+-rw-r--r--   0        0        0       75 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/utils.rst
+-rw-r--r--   0        0        0     9539 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/conf.py
+-rw-r--r--   0        0        0     2306 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/index.rst
+-rw-r--r--   0        0        0    11204 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/oauth2.rst
+-rw-r--r--   0        0        0       46 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/requirements.txt
+-rw-r--r--   0        0        0    11159 2024-05-15 23:22:07.113393 gspread-6.1.1/docs/user-guide.rst
+-rw-r--r--   0        0        0      560 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/__init__.py
+-rw-r--r--   0        0        0    14310 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/auth.py
+-rw-r--r--   0        0        0     2407 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/cell.py
+-rw-r--r--   0        0        0    16121 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/client.py
+-rw-r--r--   0        0        0     1713 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/exceptions.py
+-rw-r--r--   0        0        0    22653 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/http_client.py
+-rw-r--r--   0        0        0        0 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/py.typed
+-rw-r--r--   0        0        0    29058 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/spreadsheet.py
+-rw-r--r--   0        0        0     1287 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/urls.py
+-rw-r--r--   0        0        0    28495 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/utils.py
+-rw-r--r--   0        0        0   119486 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/worksheet.py
+-rw-r--r--   0        0        0     1512 2024-05-15 23:22:07.113393 gspread-6.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11072 1970-01-01 00:00:00.000000 gspread-6.1.1/PKG-INFO
```

### Comparing `gspread-6.1.0/HISTORY.rst` & `gspread-6.1.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,28 @@
 Release History
 ===============
 
-6.0.1 (2024-03-28)
+6.1.1 (2024-05-16)
+------------------
+
+* Add some missing typing in code by @lavigne958 in https://github.com/burnash/gspread/pull/1448
+* More fixes for `Worksheet.update` argument ordering & single cell updating (i.e. now `Worksheet.update_acell`) by @alexmalins in https://github.com/burnash/gspread/pull/1449
+* Added 'add_data_validation` to `Workhsheet` [Issue #1420] by @muddi900 in https://github.com/burnash/gspread/pull/1444
+* Bump typing-extensions from 4.10.0 to 4.11.0 by @dependabot in https://github.com/burnash/gspread/pull/1450
+* Bump black from 23.3.0 to 24.4.0 by @dependabot in https://github.com/burnash/gspread/pull/1452
+* Fix incorrect version number in HISTORY.rst from 6.0.1 to 6.1.0 by @yhay81 in https://github.com/burnash/gspread/pull/1455
+* add `get_notes` by @nbwzx in https://github.com/burnash/gspread/pull/1451
+* Bump mypy from 1.9.0 to 1.10.0 by @dependabot in https://github.com/burnash/gspread/pull/1459
+* Bump black from 24.4.0 to 24.4.2 by @dependabot in https://github.com/burnash/gspread/pull/1460
+* bugfix: handle domain name in spreadsheet copy permissions by @lavigne958 in https://github.com/burnash/gspread/pull/1458
+* Fix/api key auth version by @alifeee in https://github.com/burnash/gspread/pull/1463
+* Ignore pip vulnerabilities in CI. by @lavigne958 in https://github.com/burnash/gspread/pull/1464
+* Remove StrEnum dependency and added custom class[issue #1462] by @muddi900 in https://github.com/burnash/gspread/pull/1469
+
+6.1.0 (2024-03-28)
 ------------------
 
 * Add py.typed marker by @lavigne958 in https://github.com/burnash/gspread/pull/1422
 * Improve back-off client by @lavigne958 in https://github.com/burnash/gspread/pull/1415
 * Add new auth method API key by @lavigne958 in https://github.com/burnash/gspread/pull/1428
 * Bugfix/add set timeout by @lavigne958 in https://github.com/burnash/gspread/pull/1417
 * Fix wrapper `cast_to_a1_notation` by @lavigne958 in https://github.com/burnash/gspread/pull/1427
```

### Comparing `gspread-6.1.0/LICENSE.txt` & `gspread-6.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gspread-6.1.0/README.md` & `gspread-6.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 cell_list = worksheet.findall(criteria_re)
 ```
 
 ### Updating Cells
 
 ```python
 # Update a single cell
-worksheet.update_acell('Bingo!', 'B1')
+worksheet.update_acell('B1', 'Bingo!')
 
 # Update a range
 worksheet.update([[1, 2], [3, 4]], 'A1:B2')
 
 # Update multiple ranges at once
 worksheet.batch_update([{
     'range': 'A1:B2',
@@ -288,14 +288,38 @@
 # Get unformatted value from the same cell range
 >>> worksheet.get("A1:B2", value_render_option=ValueRenderOption.unformatted)
 [[12]]
 
 # Get formula from a cell
 >>> worksheet.get("C2:D2", value_render_option=ValueRenderOption.formula)
 [['=1/1024']]
+### Add data validation to a range
+
+```python
+import gspread
+from gspread.utils import ValidationConditionType
+
+# Restrict the input to greater than 10 in a single cell
+worksheet.add_validation(
+  'A1',
+  ValidationConditionType.number_greater,
+  [10],
+  strict=True,
+  inputMessage='Value must be greater than 10',
+)
+
+# Restrict the input to Yes/No for a specific range with dropdown
+worksheet.add_validation(
+  'C2:C7',
+   ValidationConditionType.one_of_list,
+   ['Yes',
+   'No',]
+   showCustomUi=True
+)
+
 ```
 
 ## Documentation
 
 [Documentation]\: [https://gspread.readthedocs.io/][Documentation]
 
 [Documentation]: https://gspread.readthedocs.io/en/latest/
```

### Comparing `gspread-6.1.0/docs/_templates/layout.html` & `gspread-6.1.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `gspread-6.1.0/docs/advanced.rst` & `gspread-6.1.1/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `gspread-6.1.0/docs/conf.py` & `gspread-6.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.0/docs/index.rst` & `gspread-6.1.1/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 
    gc = gspread.service_account()
 
    # Open a sheet from a spreadsheet in one go
    wks = gc.open("Where is the money Lebowski?").sheet1
 
    # Update a range of cells using the top left corner address
-   wks.update('A1', [[1, 2], [3, 4]])
+   wks.update([[1, 2], [3, 4]], 'A1')
 
    # Or update a single cell
-   wks.update('B42', "it's down there somewhere, let me take another look.")
+   wks.update_acell('B42', "it's down there somewhere, let me take another look.")
 
    # Format the header
    wks.format('A1:B1', {'textFormat': {'bold': True}})
 
 
 Getting Started
 ---------------
```

### Comparing `gspread-6.1.0/docs/oauth2.rst` & `gspread-6.1.1/docs/oauth2.rst`

 * *Files identical despite different names*

### Comparing `gspread-6.1.0/docs/user-guide.rst` & `gspread-6.1.1/docs/user-guide.rst`

 * *Files 15% similar despite different names*

```diff
@@ -298,27 +298,65 @@
 Updating Cells
 ~~~~~~~~~~~~~~
 
 Using `A1 notation <https://developers.google.com/sheets/api/guides/concepts#a1_notation>`_:
 
 .. code:: python
 
-   worksheet.update('B1', 'Bingo!')
+   worksheet.update_acell('B1', 'Bingo!')
 
 Or row and column coordinates:
 
 .. code:: python
 
    worksheet.update_cell(1, 2, 'Bingo!')
 
 Update a range
 
 .. code:: python
 
-   worksheet.update('A1:B2', [[1, 2], [3, 4]])
+   worksheet.update([[1, 2], [3, 4]], 'A1:B2')
+
+
+Adding Data Validation
+~~~~~~~~~~~~~~~~~~~~~~
+
+You can add a strict validation to a cell.
+
+.. code:: python
+
+   ws.add_validation(
+      'A1',
+      ValidationConditionType.number_greater,
+      [10],
+      strict=True,
+      inputMessage='Value must be greater than 10',
+   )
+ 
+
+Or add validation with a drop down.
+
+.. code:: python
+   
+   worksheet.add_validation(
+      'C2:C7',
+      ValidationConditionType.one_of_list,
+      ['Yes',
+      'No',]
+      showCustomUi=True
+   )
+
+
+Check out the api docs for `DataValidationRule`_ and `CondtionType`_ for more details.
+
+.. _CondtionType: https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets/other#ConditionType
+
+.. _DataValidationRule: https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets/cells#DataValidationRule 
+
+
 
 Formatting
 ~~~~~~~~~~
 
 Here's an example of basic formatting.
 
 Set **A1:B1** text format to bold:
@@ -398,9 +436,9 @@
 .. code:: python
 
    import numpy as np
 
    array = np.array([[1, 2, 3], [4, 5, 6]])
 
    # Write the array to worksheet starting from the A2 cell
-   worksheet.update('A2', array.tolist())
+   worksheet.update(array.tolist(), 'A2')
```

### Comparing `gspread-6.1.0/gspread/__init__.py` & `gspread-6.1.1/gspread/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Google Spreadsheets Python API"""
 
-__version__ = "6.1.0"
+__version__ = "6.1.1"
 __author__ = "Anton Burnashev"
 
 
 from .auth import (
     api_key,
     authorize,
     oauth,
```

### Comparing `gspread-6.1.0/gspread/auth.py` & `gspread-6.1.1/gspread/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,22 @@
 """
 
 import json
 import os
 from pathlib import Path
 from typing import Any, Dict, Iterable, Mapping, Optional, Protocol, Tuple, Union
 
-from google.auth.api_key import Credentials as APIKeyCredentials
 from google.auth.credentials import Credentials
+
+try:
+    from google.auth.api_key import Credentials as APIKeyCredentials
+
+    GOOGLE_AUTH_API_KEY_AVAILABLE = True
+except ImportError:
+    GOOGLE_AUTH_API_KEY_AVAILABLE = False
 from google.oauth2.credentials import Credentials as OAuthCredentials
 from google.oauth2.service_account import Credentials as SACredentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from requests import Session
 
 from .client import Client
 from .http_client import HTTPClient, HTTPClientType
@@ -82,16 +88,15 @@
 
 
 class FlowCallable(Protocol):
     """Protocol for OAuth flow callables."""
 
     def __call__(
         self, client_config: Mapping[str, Any], scopes: Iterable[str], port: int = 0
-    ) -> Credentials:
-        ...
+    ) -> Credentials: ...
 
 
 def local_server_flow(
     client_config: Mapping[str, Any], scopes: Iterable[str], port: int = 0
 ) -> Credentials:
     """Run an OAuth flow using a local server strategy.
 
@@ -159,15 +164,15 @@
     You can also use ``gspread.auth.READONLY_SCOPES`` for read only access.
     Obviously any method of ``gspread`` that updates a spreadsheet
     **will not work** in this case::
 
         gc = gspread.oauth(scopes=gspread.auth.READONLY_SCOPES)
 
         sh = gc.open("A spreadsheet")
-        sh.sheet1.update('A1', '42')   # <-- this will not work
+        sh.sheet1.update_acell('A1', '42')   # <-- this will not work
 
     If you're storing your user credentials in a place other than the
     default, you may provide a path to that file like so::
 
         gc = gspread.oauth(
             credentials_filename='/alternative/path/credentials.json',
             authorized_user_filename='/alternative/path/authorized_user.json',
@@ -242,15 +247,15 @@
     You can also use ``gspread.auth.READONLY_SCOPES`` for read only access.
     Obviously any method of ``gspread`` that updates a spreadsheet
     **will not work** in this case::
 
         gc = gspread.oauth_from_dict(scopes=gspread.auth.READONLY_SCOPES)
 
         sh = gc.open("A spreadsheet")
-        sh.sheet1.update('A1', '42')   # <-- this will not work
+        sh.sheet1.update_acell('A1', '42')   # <-- this will not work
 
     This function requires you to pass the credentials directly as
     a python dict. After the first authentication the function returns
     the authenticated user info, this can be passed again to authenticate
     the user without the need to run the flow again.
 
     ..
@@ -376,9 +381,14 @@
     :param http_client: A factory function that returns a client class.
         Defaults to :class:`gspread.http_client.HTTPClient` (but could also use
         :class:`gspread.http_client.BackOffHTTPClient` to avoid rate limiting)
 
     :rtype: :class:`gspread.client.Client`
 
     """
+    if GOOGLE_AUTH_API_KEY_AVAILABLE is False:
+        raise NotImplementedError(
+            "api_key is only available with package google.auth>=2.4.0."
+            'Install it with "pip install google-auth>=2.4.0".'
+        )
     creds = APIKeyCredentials(token)
     return Client(auth=creds, http_client=http_client)
```

### Comparing `gspread-6.1.0/gspread/cell.py` & `gspread-6.1.1/gspread/cell.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.0/gspread/client.py` & `gspread-6.1.1/gspread/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,17 @@
         self,
         auth: Credentials,
         session: Optional[Session] = None,
         http_client: HTTPClientType = HTTPClient,
     ) -> None:
         self.http_client = http_client(auth, session)
 
-    def set_timeout(self, timeout: Optional[Union[float, Tuple[float, float]]] = None):
+    def set_timeout(
+        self, timeout: Optional[Union[float, Tuple[float, float]]] = None
+    ) -> None:
         """How long to wait for the server to send
         data before giving up, as a float, or a ``(connect timeout,
         read timeout)`` tuple.
 
         Use value ``None`` to restore default timeout
 
         Value for ``timeout`` is in seconds (s).
@@ -72,15 +74,15 @@
 
         :returns: a list of dicts containing the keys id, name, createdTime and modifiedTime.
         """
         files, _ = self._list_spreadsheet_files(title=title, folder_id=folder_id)
         return files
 
     def _list_spreadsheet_files(
-        self, title=None, folder_id=None
+        self, title: Optional[str] = None, folder_id: Optional[str] = None
     ) -> Tuple[List[Dict[str, Any]], Response]:
         files = []
         page_token = ""
         url = DRIVE_FILES_API_V3_URL
 
         query = f'mimeType="{MimeType.google_sheets}"'
         if title:
@@ -311,18 +313,28 @@
             original = self.open_by_key(file_id)
 
             permissions = original.list_permissions()
             for p in permissions:
                 if p.get("deleted"):
                     continue
 
+                # In case of domain type the domain extract the domain
+                # In case of user/group extract the emailAddress
+                # Otherwise use None for type 'Anyone'
+
+                email_or_domain = ""
+                if str(p["type"]) == "domain":
+                    email_or_domain = str(p["domain"])
+                elif str(p["type"]) in ("user", "group"):
+                    email_or_domain = str(p["emailAddress"])
+
                 new_spreadsheet.share(
-                    email_address=p["emailAddress"],
-                    perm_type=p["type"],
-                    role=p["role"],
+                    email_address=email_or_domain,
+                    perm_type=str(p["type"]),
+                    role=str(p["role"]),
                     notify=False,
                 )
 
         if copy_comments is True:
             source_url = DRIVE_FILES_API_V3_COMMENTS_URL % (file_id)
             page_token = ""
             comments = []
```

### Comparing `gspread-6.1.0/gspread/exceptions.py` & `gspread-6.1.1/gspread/exceptions.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.0/gspread/http_client.py` & `gspread-6.1.1/gspread/http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,15 +280,17 @@
         """Lower-level method that directly calls `spreadsheets.sheets.copyTo <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.sheets/copyTo>`_."""
         url = SPREADSHEET_SHEETS_COPY_TO_URL % (id, sheet_id)
 
         body = {"destinationSpreadsheetId": destination_spreadsheet_id}
         r = self.request("post", url, json=body)
         return r.json()
 
-    def fetch_sheet_metadata(self, id: str, params: Optional[ParamsType] = None) -> Any:
+    def fetch_sheet_metadata(
+        self, id: str, params: Optional[ParamsType] = None
+    ) -> Mapping[str, Any]:
         """Similar to :method spreadsheets_get:`gspread.http_client.spreadsheets_get`,
         get the spreadsheet form the API but by default **does not get the cells data**.
         It only retrieve the the metadata from the spreadsheet.
 
         :param str id: the spreadsheet ID key
         :param dict params: (optional) the HTTP params for the GET request.
             By default sets the parameter ``includeGridData`` to ``false``.
```

### Comparing `gspread-6.1.0/gspread/spreadsheet.py` & `gspread-6.1.1/gspread/spreadsheet.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,161 +3,177 @@
 ~~~~~~~~~~~~~~
 
 This module contains common spreadsheets' models.
 
 """
 
 import warnings
-from typing import Any, Dict, Union
+from typing import Any, Dict, Generator, Iterable, List, Mapping, Optional, Union
 
+from requests import Response
+
+from .cell import Cell
 from .exceptions import WorksheetNotFound
-from .http_client import HTTPClient
+from .http_client import HTTPClient, ParamsType
 from .urls import DRIVE_FILES_API_V3_URL, SPREADSHEET_DRIVE_URL
 from .utils import ExportFormat, finditem
 from .worksheet import Worksheet
 
 
 class Spreadsheet:
     """The class that represents a spreadsheet."""
 
-    def __init__(self, http_client: HTTPClient, properties: Dict[str, Any]):
+    def __init__(self, http_client: HTTPClient, properties: Dict[str, Union[str, Any]]):
         self.client = http_client
         self._properties = properties
 
         metadata = self.fetch_sheet_metadata()
         self._properties.update(metadata["properties"])
 
     @property
-    def id(self):
+    def id(self) -> str:
         """Spreadsheet ID."""
         return self._properties["id"]
 
     @property
-    def title(self):
+    def title(self) -> str:
         """Spreadsheet title."""
         return self._properties["title"]
 
     @property
-    def url(self):
+    def url(self) -> str:
         """Spreadsheet URL."""
         return SPREADSHEET_DRIVE_URL % self.id
 
     @property
-    def creationTime(self):
+    def creationTime(self) -> str:
         """Spreadsheet Creation time."""
         if "createdTime" not in self._properties:
             self.update_drive_metadata()
         return self._properties["createdTime"]
 
     @property
-    def lastUpdateTime(self):
+    def lastUpdateTime(self) -> str:
         """Spreadsheet last updated time.
         Only updated on initialisation.
         For actual last updated time, use get_lastUpdateTime()."""
         warnings.warn(
             "worksheet.lastUpdateTime is deprecated, please use worksheet.get_lastUpdateTime()",
             category=DeprecationWarning,
         )
         if "modifiedTime" not in self._properties:
             self.update_drive_metadata()
         return self._properties["modifiedTime"]
 
     @property
-    def timezone(self):
+    def timezone(self) -> str:
         """Spreadsheet timeZone"""
         return self._properties["timeZone"]
 
     @property
-    def locale(self):
+    def locale(self) -> str:
         """Spreadsheet locale"""
         return self._properties["locale"]
 
     @property
-    def sheet1(self):
+    def sheet1(self) -> Worksheet:
         """Shortcut property for getting the first worksheet."""
         return self.get_worksheet(0)
 
-    def __iter__(self):
+    def __iter__(self) -> Generator[Worksheet, None, None]:
         yield from self.worksheets()
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<{} {} id:{}>".format(
             self.__class__.__name__,
             repr(self.title),
             self.id,
         )
 
-    def batch_update(self, body):
+    def batch_update(self, body: Mapping[str, Any]) -> Any:
         """Lower-level method that directly calls `spreadsheets/<ID>:batchUpdate <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets/batchUpdate>`_.
 
         :param dict body: `Batch Update Request body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets/batchUpdate#request-body>`_.
         :returns: `Batch Update Response body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets/batchUpdate#response-body>`_.
         :rtype: dict
 
         .. versionadded:: 3.0
         """
         return self.client.batch_update(self.id, body)
 
-    def values_append(self, range, params, body):
+    def values_append(
+        self, range: str, params: ParamsType, body: Mapping[str, Any]
+    ) -> Any:
         """Lower-level method that directly calls `spreadsheets/<ID>/values:append <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/append>`_.
 
         :param str range: The `A1 notation <https://developers.google.com/sheets/api/guides/concepts#a1_notation>`_
                           of a range to search for a logical table of data. Values will be appended after the last row of the table.
         :param dict params: `Values Append Query parameters <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/append#query-parameters>`_.
         :param dict body: `Values Append Request body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/append#request-body>`_.
         :returns: `Values Append Response body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/append#response-body>`_.
         :rtype: dict
 
         .. versionadded:: 3.0
         """
         return self.client.values_append(self.id, range, params, body)
 
-    def values_clear(self, range):
+    def values_clear(self, range: str) -> Any:
         """Lower-level method that directly calls `spreadsheets/<ID>/values:clear <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/clear>`_.
 
         :param str range: The `A1 notation <https://developers.google.com/sheets/api/guides/concepts#a1_notation>`_ of the values to clear.
         :returns: `Values Clear Response body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/clear#response-body>`_.
         :rtype: dict
 
         .. versionadded:: 3.0
         """
         return self.client.values_clear(self.id, range)
 
-    def values_batch_clear(self, params=None, body=None):
+    def values_batch_clear(
+        self,
+        params: Optional[ParamsType] = None,
+        body: Optional[Mapping[str, Any]] = None,
+    ) -> Any:
         """Lower-level method that directly calls `spreadsheets/<ID>/values:batchClear`
 
         :param dict params: (optional) `Values Batch Clear Query parameters <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/batchClear#path-parameters>`_.
         :param dict body: (optional) `Values Batch Clear request body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/batchClear#request-body>`_.
         :rtype: dict
         """
         return self.client.values_batch_clear(self.id, params, body)
 
-    def values_get(self, range, params=None):
+    def values_get(self, range: str, params: Optional[ParamsType] = None) -> Any:
         """Lower-level method that directly calls `GET spreadsheets/<ID>/values/<range> <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/get>`_.
 
         :param str range: The `A1 notation <https://developers.google.com/sheets/api/guides/concepts#a1_notation>`_ of the values to retrieve.
         :param dict params: (optional) `Values Get Query parameters <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/get#query-parameters>`_.
         :returns: `Values Get Response body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/get#response-body>`_.
         :rtype: dict
 
         .. versionadded:: 3.0
         """
         return self.client.values_get(self.id, range, params=params)
 
-    def values_batch_get(self, ranges, params=None):
+    def values_batch_get(
+        self, ranges: List[str], params: Optional[ParamsType] = None
+    ) -> Any:
         """Lower-level method that directly calls `spreadsheets/<ID>/values:batchGet <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/batchGet>`_.
 
         :param list ranges: List of ranges in the `A1 notation <https://developers.google.com/sheets/api/guides/concepts#a1_notation>`_ of the values to retrieve.
         :param dict params: (optional) `Values Batch Get Query parameters <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/batchGet#query-parameters>`_.
         :returns: `Values Batch Get Response body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/batchGet#response-body>`_.
         :rtype: dict
         """
         return self.client.values_batch_get(self.id, ranges, params=params)
 
-    def values_update(self, range, params=None, body=None):
+    def values_update(
+        self,
+        range: str,
+        params: Optional[ParamsType] = None,
+        body: Optional[Mapping[str, Any]] = None,
+    ) -> Any:
         """Lower-level method that directly calls `PUT spreadsheets/<ID>/values/<range> <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/update>`_.
 
         :param str range: The `A1 notation <https://developers.google.com/sheets/api/guides/concepts#a1_notation>`_ of the values to update.
         :param dict params: (optional) `Values Update Query parameters <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/update#query-parameters>`_.
         :param dict body: (optional) `Values Update Request body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/update#request-body>`_.
         :returns: `Values Update Response body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/update#response-body>`_.
         :rtype: dict
@@ -174,46 +190,50 @@
                 }
             )
 
         .. versionadded:: 3.0
         """
         return self.client.values_update(self.id, range, params=params, body=body)
 
-    def values_batch_update(self, body=None):
+    def values_batch_update(self, body: Optional[Mapping[str, Any]] = None) -> Any:
         """Lower-level method that directly calls `spreadsheets/<ID>/values:batchUpdate <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/batchUpdate>`_.
 
         :param dict body: (optional) `Values Batch Update Request body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/batchUpdate#request-body>`_.
         :returns: `Values Batch Update Response body <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.values/batchUpdate#response-body>`_.
         :rtype: dict
         """
         return self.client.values_batch_update(self.id, body=body)
 
-    def _spreadsheets_get(self, params=None):
+    def _spreadsheets_get(self, params: Optional[ParamsType] = None) -> Any:
         """A method stub that directly calls `spreadsheets.get <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets/get>`_."""
         return self.client.spreadsheets_get(self.id, params=params)
 
-    def _spreadsheets_sheets_copy_to(self, sheet_id, destination_spreadsheet_id):
+    def _spreadsheets_sheets_copy_to(
+        self, sheet_id: int, destination_spreadsheet_id: str
+    ) -> Any:
         """Lower-level method that directly calls `spreadsheets.sheets.copyTo <https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets.sheets/copyTo>`_."""
         return self.client.spreadsheets_sheets_copy_to(
             self.id, sheet_id, destination_spreadsheet_id
         )
 
-    def fetch_sheet_metadata(self, params=None):
+    def fetch_sheet_metadata(
+        self, params: Optional[ParamsType] = None
+    ) -> Mapping[str, Any]:
         """Similar to :method spreadsheets_get:`gspread.http_client.spreadsheets_get`,
         get the spreadsheet form the API but by default **does not get the cells data**.
         It only retrieve the the metadata from the spreadsheet.
 
         :param dict params: (optional) the HTTP params for the GET request.
             By default sets the parameter ``includeGridData`` to ``false``.
         :returns: The raw spreadsheet
         :rtype: dict
         """
         return self.client.fetch_sheet_metadata(self.id, params=params)
 
-    def get_worksheet(self, index):
+    def get_worksheet(self, index: int) -> Worksheet:
         """Returns a worksheet with specified `index`.
 
         :param index: An index of a worksheet. Indexes start from zero.
         :type index: int
 
         :returns: an instance of :class:`gspread.worksheet.Worksheet`.
 
@@ -229,15 +249,15 @@
 
         try:
             properties = sheet_data["sheets"][index]["properties"]
             return Worksheet(self, properties, self.id, self.client)
         except (KeyError, IndexError):
             raise WorksheetNotFound("index {} not found".format(index))
 
-    def get_worksheet_by_id(self, id: Union[str, int]):
+    def get_worksheet_by_id(self, id: Union[str, int]) -> Worksheet:
         """Returns a worksheet with specified `worksheet id`.
 
         :param id: The id of a worksheet. it can be seen in the url as the value of the parameter 'gid'.
         :type id: str | int
 
         :returns: an instance of :class:`gspread.worksheet.Worksheet`.
         :raises:
@@ -260,15 +280,15 @@
                 lambda x: x["properties"]["sheetId"] == worksheet_id_int,
                 sheet_data["sheets"],
             )
             return Worksheet(self, item["properties"], self.id, self.client)
         except (StopIteration, KeyError):
             raise WorksheetNotFound("id {} not found".format(worksheet_id_int))
 
-    def worksheets(self, exclude_hidden: bool = False):
+    def worksheets(self, exclude_hidden: bool = False) -> List[Worksheet]:
         """Returns a list of all :class:`worksheets <gspread.worksheet.Worksheet>`
         in a spreadsheet.
 
         :param exclude_hidden: (optional) If set to ``True`` will only return
                                  visible worksheets. Default is ``False``.
         :type exclude_hidden: bool
 
@@ -280,15 +300,15 @@
             Worksheet(self, s["properties"], self.id, self.client)
             for s in sheet_data["sheets"]
         ]
         if exclude_hidden:
             worksheets = [w for w in worksheets if not w.isSheetHidden]
         return worksheets
 
-    def worksheet(self, title):
+    def worksheet(self, title: str) -> Worksheet:
         """Returns a worksheet with specified `title`.
 
         :param title: A title of a worksheet. If there're multiple
                       worksheets with the same title, first one will
                       be returned.
         :type title: str
 
@@ -308,29 +328,33 @@
                 lambda x: x["properties"]["title"] == title,
                 sheet_data["sheets"],
             )
             return Worksheet(self, item["properties"], self.id, self.client)
         except (StopIteration, KeyError):
             raise WorksheetNotFound(title)
 
-    def add_worksheet(self, title, rows, cols, index=None):
+    def add_worksheet(
+        self, title: str, rows: int, cols: int, index: Optional[int] = None
+    ) -> Worksheet:
         """Adds a new worksheet to a spreadsheet.
 
         :param title: A title of a new worksheet.
         :type title: str
         :param rows: Number of rows.
         :type rows: int
         :param cols: Number of columns.
         :type cols: int
         :param index: Position of the sheet.
         :type index: int
 
         :returns: a newly created :class:`worksheets <gspread.worksheet.Worksheet>`.
         """
-        body = {
+        body: Dict[
+            str, List[Dict[str, Dict[str, Dict[str, Union[str, int, Dict[str, int]]]]]]
+        ] = {
             "requests": [
                 {
                     "addSheet": {
                         "properties": {
                             "title": title,
                             "sheetType": "GRID",
                             "gridProperties": {
@@ -350,19 +374,19 @@
 
         properties = data["replies"][0]["addSheet"]["properties"]
 
         return Worksheet(self, properties, self.id, self.client)
 
     def duplicate_sheet(
         self,
-        source_sheet_id,
-        insert_sheet_index=None,
-        new_sheet_id=None,
-        new_sheet_name=None,
-    ):
+        source_sheet_id: int,
+        insert_sheet_index: Optional[int] = None,
+        new_sheet_id: Optional[int] = None,
+        new_sheet_name: Optional[str] = None,
+    ) -> Worksheet:
         """Duplicates the contents of a sheet.
 
         :param int source_sheet_id: The sheet ID to duplicate.
         :param int insert_sheet_index: (optional) The zero-based index
                                        where the new sheet should be inserted.
                                        The index of all sheets after this are
                                        incremented.
@@ -384,38 +408,40 @@
             source_sheet_id,
             self,
             insert_sheet_index=insert_sheet_index,
             new_sheet_id=new_sheet_id,
             new_sheet_name=new_sheet_name,
         )
 
-    def del_worksheet(self, worksheet):
+    def del_worksheet(self, worksheet: Worksheet) -> Any:
         """Deletes a worksheet from a spreadsheet.
 
         :param worksheet: The worksheet to be deleted.
         :type worksheet: :class:`~gspread.worksheet.Worksheet`
         """
         body = {"requests": [{"deleteSheet": {"sheetId": worksheet.id}}]}
 
         return self.client.batch_update(self.id, body)
 
-    def del_worksheet_by_id(self, worksheet_id: Union[str, int]):
+    def del_worksheet_by_id(self, worksheet_id: Union[str, int]) -> Any:
         """
         Deletes a Worksheet by id
         """
         try:
             worksheet_id_int = int(worksheet_id)
         except ValueError as ex:
             raise ValueError("id should be int") from ex
 
         body = {"requests": [{"deleteSheet": {"sheetId": worksheet_id_int}}]}
 
         return self.client.batch_update(self.id, body)
 
-    def reorder_worksheets(self, worksheets_in_desired_order):
+    def reorder_worksheets(
+        self, worksheets_in_desired_order: Iterable[Worksheet]
+    ) -> Any:
         """Updates the ``index`` property of each Worksheet to reflect
         its index in the provided sequence of Worksheets.
 
         :param worksheets_in_desired_order: Iterable of Worksheet objects in desired order.
 
         Note: If you omit some of the Spreadsheet's existing Worksheet objects from
         the provided sequence, those Worksheets will be appended to the end of the sequence
@@ -444,21 +470,21 @@
             ]
         }
 
         return self.client.batch_update(self.id, body)
 
     def share(
         self,
-        email_address,
-        perm_type,
-        role,
-        notify=True,
-        email_message=None,
-        with_link=False,
-    ):
+        email_address: str,
+        perm_type: str,
+        role: str,
+        notify: bool = True,
+        email_message: Optional[str] = None,
+        with_link: bool = False,
+    ) -> Response:
         """Share the spreadsheet with other accounts.
 
         :param email_address: user or group e-mail address, domain name
                       or None for 'anyone' type.
         :type email_address: str, None
         :param perm_type: The account type.
                Allowed values are: ``user``, ``group``, ``domain``,
@@ -488,15 +514,15 @@
             perm_type=perm_type,
             role=role,
             notify=notify,
             email_message=email_message,
             with_link=with_link,
         )
 
-    def export(self, format=ExportFormat.PDF):
+    def export(self, format: ExportFormat = ExportFormat.PDF) -> bytes:
         """Export the spreadsheet in the given format.
 
         :param str file_id: A key of a spreadsheet to export
 
         :param format: The format of the resulting file.
             Possible values are:
 
@@ -513,19 +539,19 @@
 
         :returns bytes: The content of the exported file.
 
         .. _ExportFormat: https://developers.google.com/drive/api/guides/ref-export-formats
         """
         return self.client.export(self.id, format)
 
-    def list_permissions(self):
+    def list_permissions(self) -> List[Dict[str, Union[str, bool]]]:
         """Lists the spreadsheet's permissions."""
         return self.client.list_permissions(self.id)
 
-    def remove_permissions(self, value, role="any"):
+    def remove_permissions(self, value: str, role: str = "any") -> List[str]:
         """Remove permissions from a user or domain.
 
         :param value: User or domain to remove permissions from
         :type value: str
         :param role: (optional) Permission to remove. Defaults to all
                      permissions.
         :type role: str
@@ -538,26 +564,26 @@
             # Remove all Otto's permissions for this spreadsheet
             sh.remove_permissions('otto@example.com')
         """
         permission_list = self.client.list_permissions(self.id)
 
         key = "emailAddress" if "@" in value else "domain"
 
-        filtered_id_list = [
-            p["id"]
+        filtered_id_list: List[str] = [
+            str(p["id"])
             for p in permission_list
             if p.get(key) == value and (p["role"] == role or role == "any")
         ]
 
         for permission_id in filtered_id_list:
             self.client.remove_permission(self.id, permission_id)
 
         return filtered_id_list
 
-    def transfer_ownership(self, permission_id):
+    def transfer_ownership(self, permission_id: str) -> Response:
         """Transfer the ownership of this file to a new user.
 
         It is necessary to first create the permission with the new owner's email address,
         get the permission ID then use this method to transfer the ownership.
 
         .. note::
 
@@ -577,15 +603,15 @@
             # new owner must be writer in order to accept ownership by editing permissions
             "role": "writer",
             "pendingOwner": True,
         }
 
         return self.client.request("patch", url, json=payload)
 
-    def accept_ownership(self, permission_id):
+    def accept_ownership(self, permission_id: str) -> Response:
         """Accept the pending ownership request on that file.
 
         It is necessary to edit the permission with the pending ownership.
 
         .. note::
 
            You can only accept ownership transfer for the user currently being used.
@@ -597,39 +623,39 @@
             permission_id,
         )
 
         payload = {
             "role": "owner",
         }
 
-        params = {
+        params: ParamsType = {
             "transferOwnership": True,
         }
 
         return self.client.request("patch", url, json=payload, params=params)
 
-    def named_range(self, named_range):
+    def named_range(self, named_range: str) -> List[Cell]:
         """return a list of :class:`gspread.cell.Cell` objects from
         the specified named range.
 
         :param named_range: A string with a named range value to fetch.
         :type named_range: str
         """
 
         # the function `range` does all necessary actions to get a named range.
         # This is only here to provide better user experience.
         return self.sheet1.range(named_range)
 
-    def list_named_ranges(self):
+    def list_named_ranges(self) -> List[Any]:
         """Lists the spreadsheet's named ranges."""
         return self.fetch_sheet_metadata(params={"fields": "namedRanges"}).get(
             "namedRanges", []
         )
 
-    def update_title(self, title):
+    def update_title(self, title: str) -> Any:
         """Renames the spreadsheet.
 
         :param str title: A new title.
         """
         body = {
             "requests": [
                 {
@@ -641,15 +667,15 @@
             ]
         }
 
         res = self.batch_update(body)
         self._properties["title"] = title
         return res
 
-    def update_timezone(self, timezone):
+    def update_timezone(self, timezone: str) -> Any:
         """Updates the current spreadsheet timezone.
         Can be any timezone in CLDR format such as "America/New_York"
         or a custom time zone such as GMT-07:00.
         """
 
         body = {
             "requests": [
@@ -662,15 +688,15 @@
             ]
         }
 
         res = self.batch_update(body)
         self._properties["timeZone"] = timezone
         return res
 
-    def update_locale(self, locale):
+    def update_locale(self, locale: str) -> Any:
         """Update the locale of the spreadsheet.
         Can be any of the ISO 639-1 language codes, such as: de, fr, en, ...
         Or an ISO 639-2 if no ISO 639-1 exists.
         Or a combination of the ISO language code and country code,
         such as en_US, de_CH, fr_FR, ...
 
         .. note::
@@ -688,17 +714,17 @@
             ]
         }
 
         res = self.batch_update(body)
         self._properties["locale"] = locale
         return res
 
-    def list_protected_ranges(self, sheetid):
+    def list_protected_ranges(self, sheetid: int) -> List[Any]:
         """Lists the spreadsheet's protected named ranges"""
-        sheets = self.fetch_sheet_metadata(
+        sheets: List[Mapping[str, Any]] = self.fetch_sheet_metadata(
             params={"fields": "sheets.properties,sheets.protectedRanges"}
         )["sheets"]
 
         try:
             sheet = finditem(
                 lambda sheet: sheet["properties"]["sheetId"] == sheetid, sheets
             )
```

### Comparing `gspread-6.1.0/gspread/urls.py` & `gspread-6.1.1/gspread/urls.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.0/gspread/utils.py` & `gspread-6.1.1/gspread/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 gspread.utils
 ~~~~~~~~~~~~~
 
 This module contains utility functions.
 
 """
 
+import enum
 import re
 from collections import defaultdict
 from collections.abc import Sequence
 from functools import wraps
 from itertools import chain
 from typing import (
     TYPE_CHECKING,
@@ -26,15 +27,14 @@
     Union,
 )
 from urllib.parse import quote as uquote
 
 from google.auth.credentials import Credentials as Credentials
 from google.oauth2.credentials import Credentials as UserCredentials
 from google.oauth2.service_account import Credentials as ServiceAccountCredentials
-from strenum import StrEnum
 
 from .exceptions import IncorrectCellLabel, InvalidInputValue, NoValidUrlKeyFound
 
 if TYPE_CHECKING:
     from .cell import Cell
 
 
@@ -43,14 +43,29 @@
 A1_ADDR_ROW_COL_RE = re.compile(r"([A-Za-z]+)?([1-9]\d*)?$")
 A1_ADDR_FULL_RE = re.compile(r"[A-Za-z]+\d+:[A-Za-z]+\d+")  # e.g. A1:B2 not A1:B
 
 URL_KEY_V1_RE = re.compile(r"key=([^&#]+)")
 URL_KEY_V2_RE = re.compile(r"/spreadsheets/d/([a-zA-Z0-9-_]+)")
 
 
+class StrEnum(str, enum.Enum):
+    def __new__(cls, value, *args, **kwargs):
+        if not isinstance(value, (str, enum.auto)):
+            raise TypeError(
+                f"Values of StrEnums must be strings: {value!r} is a {type(value)}"
+            )
+        return super().__new__(cls, value, *args, **kwargs)
+
+    def __str__(self):
+        return str(self.value)
+
+    def _generate_next_value_(name, *_):
+        return name
+
+
 class Dimension(StrEnum):
     rows = "ROWS"
     cols = "COLUMNS"
 
 
 class MergeType(StrEnum):
     merge_all = "MERGE_ALL"
@@ -114,14 +129,49 @@
 
 
 class GridRangeType(StrEnum):
     ValueRange = "ValueRange"
     ListOfLists = "ListOfLists"
 
 
+class ValidationConditionType(StrEnum):
+    number_greater = "NUMBER_GREATER"
+    number_greater_than_eq = "NUMBER_GREATER_THAN_EQ"
+    number_less = "NUMBER_LESS"
+    number_less_than_eq = "NUMBER_LESS_THAN_EQ"
+    number_eq = "NUMBER_EQ"
+    number_not_eq = "NUMBER_NOT_EQ"
+    number_between = "NUMBER_BETWEEN"
+    number_not_between = "NUMBER_NOT_BETWEEN"
+    text_contains = "TEXT_CONTAINS"
+    text_not_contains = "TEXT_NOT_CONTAINS"
+    text_starts_with = "TEXT_STARTS_WITH"
+    text_ends_with = "TEXT_ENDS_WITH"
+    text_eq = "TEXT_EQ"
+    text_is_email = "TEXT_IS_EMAIL"
+    text_is_url = "TEXT_IS_URL"
+    date_eq = "DATE_EQ"
+    date_before = "DATE_BEFORE"
+    date_after = "DATE_AFTER"
+    date_on_or_before = "DATE_ON_OR_BEFORE"
+    date_on_or_after = "DATE_ON_OR_AFTER"
+    date_between = "DATE_BETWEEN"
+    date_not_between = "DATE_NOT_BETWEEN"
+    date_is_valid = "DATE_IS_VALID"
+    one_of_range = "ONE_OF_RANGE"
+    one_of_list = "ONE_OF_LIST"
+    blank = "BLANK"
+    not_blank = "NOT_BLANK"
+    custom_formula = "CUSTOM_FORMULA"
+    boolean = "BOOLEAN"
+    text_not_eq = "TEXT_NOT_EQ"
+    date_not_eq = "DATE_NOT_EQ"
+    filter_expression = "FILTER_EXPRESSION"
+
+
 def convert_credentials(credentials: Credentials) -> Credentials:
     module = credentials.__module__
     cls = credentials.__class__.__name__
     if "oauth2client" in module and cls == "ServiceAccountCredentials":
         return _convert_service_account(credentials)
     elif "oauth2client" in module and cls in (
         "OAuth2Credentials",
@@ -240,15 +290,15 @@
                     else:
                         numericised = default_blank
 
     return numericised
 
 
 def numericise_all(
-    values: List[Optional[AnyStr]],
+    values: List[AnyStr],
     empty2zero: bool = False,
     default_blank: Any = "",
     allow_underscores_in_numeric_literals: bool = False,
     ignore: List[int] = [],
 ) -> List[Optional[Union[int, float, AnyStr]]]:
     """Returns a list of numericised values from strings except those from the
     row specified as ignore.
@@ -517,15 +567,15 @@
         raise InvalidInputValue(
             "invalid value: {}, must be a column letter".format(column)
         )
 
     return index
 
 
-def cast_to_a1_notation(method: Callable[..., Any]) -> Callable[..., Any]:
+def cast_to_a1_notation(method: Callable[..., T]) -> Callable[..., T]:
     """Decorator function casts wrapped arguments to A1 notation in range
     method calls.
     """
 
     def contains_row_cols(args: Tuple[Any, ...]) -> bool:
         return (
             isinstance(args[0], int)
@@ -705,15 +755,20 @@
 
     >>> is_scalar(set())
     True
     """
     return isinstance(x, str) or not isinstance(x, Sequence)
 
 
-def combined_merge_values(worksheet_metadata, values, start_row_index, start_col_index):
+def combined_merge_values(
+    worksheet_metadata: Mapping[str, Any],
+    values: List[List[Any]],
+    start_row_index: int,
+    start_col_index: int,
+) -> List[List[Any]]:
     """For each merged region, replace all values with the value of the top-left cell of the region.
     e.g., replaces
     [
     [1, None, None],
     [None, None, None],
     ]
     with
@@ -729,14 +784,17 @@
     :param values: The values returned by the Google API for the worksheet. 2D array.
 
     :param start_row_index: The index of the first row of the values in the worksheet.
         e.g., if the values are in rows 3-5, this should be 2.
 
     :param start_col_index: The index of the first column of the values in the worksheet.
         e.g., if the values are in columns C-E, this should be 2.
+
+    :returns: matrix of values with merged coordinates filled according to top-left value
+    :rtype: list(list(any))
     """
     merges = worksheet_metadata.get("merges", [])
     # each merge has "startRowIndex", "endRowIndex", "startColumnIndex", "endColumnIndex
     new_values = [list(row) for row in values]
 
     # max row and column indices
     max_row_index = len(values) - 1
```

### Comparing `gspread-6.1.0/gspread/worksheet.py` & `gspread-6.1.1/gspread/worksheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     Dimension,
     GridRangeType,
     InsertDataOption,
     MergeType,
     PasteOrientation,
     PasteType,
     T,
+    ValidationConditionType,
     ValueInputOption,
     ValueRenderOption,
     a1_range_to_grid_range,
     a1_to_rowcol,
     absolute_range_name,
     cast_to_a1_notation,
     cell_list_to_rect,
@@ -110,15 +111,15 @@
 
     .. note::
 
        This class should never be instantiated manually.
        It will be instantiated using the response from the sheet API.
     """
 
-    _json: MutableMapping[str, Any] = {}
+    _json: MutableMapping[str, str] = {}
 
     @classmethod
     def from_json(cls: Type[ValueRangeType], json: Mapping[str, Any]) -> ValueRangeType:
         values = json.get("values", [])
         new_obj = cls(values)
         new_obj._json = {
             "range": json["range"],
@@ -445,15 +446,15 @@
         major_dimension: Optional[Dimension] = None,
         value_render_option: Optional[ValueRenderOption] = None,
         date_time_render_option: Optional[DateTimeOption] = None,
         combine_merged_cells: bool = False,
         maintain_size: bool = False,
         pad_values: bool = True,
         return_type: GridRangeType = GridRangeType.ListOfLists,
-    ) -> List[List[T]]:
+    ) -> Union[ValueRange, List[List[Any]]]:
         """Alias for :meth:`~gspread.worksheet.Worksheet.get`...
 
         with ``return_type`` set to ``List[List[Any]]``
         and ``pad_values`` set to ``True``
         (legacy method)
         """
         return self.get(
@@ -473,36 +474,36 @@
         major_dimension: Optional[Dimension] = None,
         value_render_option: Optional[ValueRenderOption] = None,
         date_time_render_option: Optional[DateTimeOption] = None,
         combine_merged_cells: bool = False,
         maintain_size: bool = False,
         pad_values: bool = True,
         return_type: GridRangeType = GridRangeType.ListOfLists,
-    ) -> List[List[T]]:
+    ) -> Union[ValueRange, List[List[Any]]]:
         """Alias to :meth:`~gspread.worksheet.Worksheet.get_values`"""
         return self.get_values(
             range_name=range_name,
             major_dimension=major_dimension,
             value_render_option=value_render_option,
             date_time_render_option=date_time_render_option,
             combine_merged_cells=combine_merged_cells,
             maintain_size=maintain_size,
             pad_values=pad_values,
             return_type=return_type,
         )
 
     def get_all_records(
         self,
-        head=1,
-        expected_headers=None,
-        value_render_option=None,
-        default_blank="",
-        numericise_ignore=[],
-        allow_underscores_in_numeric_literals=False,
-        empty2zero=False,
+        head: int = 1,
+        expected_headers: Optional[List[str]] = None,
+        value_render_option: Optional[ValueRenderOption] = None,
+        default_blank: str = "",
+        numericise_ignore: Iterable[Union[str, int]] = [],
+        allow_underscores_in_numeric_literals: bool = False,
+        empty2zero: bool = False,
     ) -> List[Dict[str, Union[int, float, str]]]:
         """Returns a list of dictionaries, all of them having the contents of
         the spreadsheet with the head row as keys and each of these
         dictionaries holding the contents of subsequent rows of cells as
         values.
 
         This method uses the function :func:`gspread.utils.to_records` to build the resulting
@@ -594,15 +595,15 @@
         else:
             values = [
                 numericise_all(
                     row,
                     empty2zero,
                     default_blank,
                     allow_underscores_in_numeric_literals,
-                    numericise_ignore,
+                    numericise_ignore,  # type: ignore
                 )
                 for row in values
             ]
 
         return to_records(keys, values)
 
     def get_all_cells(self) -> List[Cell]:
@@ -612,15 +613,15 @@
 
     def row_values(
         self,
         row: int,
         major_dimension: Optional[Dimension] = None,
         value_render_option: Optional[ValueRenderOption] = None,
         date_time_render_option: Optional[DateTimeOption] = None,
-    ) -> List[Optional[Union[int, float, str]]]:
+    ) -> List[str]:
         """Returns a list of all values in a `row`.
 
         Empty cells in this list will be rendered as :const:`None`.
 
         :param int row: Row number (one-based).
 
         :param str major_dimension: (optional) The major dimension of the
@@ -822,15 +823,15 @@
         major_dimension: Optional[Dimension] = None,
         value_render_option: Optional[ValueRenderOption] = None,
         date_time_render_option: Optional[DateTimeOption] = None,
         combine_merged_cells: bool = False,
         maintain_size: bool = False,
         pad_values: bool = False,
         return_type: GridRangeType = GridRangeType.ValueRange,
-    ) -> Union[ValueRange, List[List[Any]]]:
+    ) -> Union[ValueRange, List[List[str]]]:
         """Reads values of a single range or a cell of a sheet.
 
         Returns a ValueRange (list of lists) containing all values from a specified range or cell
 
         By default values are returned as strings. See ``value_render_option``
         to change the default format.
 
@@ -2087,20 +2088,22 @@
                 {
                     "addProtectedRange": {
                         "protectedRange": {
                             "range": grid_range,
                             "description": description,
                             "warningOnly": warning_only,
                             "requestingUserCanEdit": requesting_user_can_edit,
-                            "editors": None
-                            if warning_only
-                            else {
-                                "users": editor_users_emails,
-                                "groups": editor_groups_emails,
-                            },
+                            "editors": (
+                                None
+                                if warning_only
+                                else {
+                                    "users": editor_users_emails,
+                                    "groups": editor_groups_emails,
+                                }
+                            ),
                         }
                     }
                 }
             ]
         }
 
         return self.client.batch_update(self.spreadsheet_id, body)
@@ -2391,15 +2394,15 @@
         if rows is not None:
             self._properties["gridProperties"]["frozenRowCount"] = rows
         if cols is not None:
             self._properties["gridProperties"]["frozenColumnCount"] = cols
         return res
 
     @cast_to_a1_notation
-    def set_basic_filter(self, name: Optional[str] = None):
+    def set_basic_filter(self, name: Optional[str] = None) -> Any:
         """Add a basic filter to the worksheet. If a range or boundaries
         are passed, the filter will be limited to the given range.
 
         :param str name: A string with range value in A1 notation,
             e.g. ``A1:A5``.
 
         Alternatively, you may specify numeric boundaries. All values
@@ -2534,15 +2537,15 @@
         :rtype: dict
         """
         return self.client.spreadsheets_sheets_copy_to(
             self.spreadsheet_id, self.id, destination_spreadsheet_id
         )
 
     @cast_to_a1_notation
-    def merge_cells(self, name: str, merge_type: str = MergeType.merge_all):
+    def merge_cells(self, name: str, merge_type: str = MergeType.merge_all) -> Any:
         """Merge cells.
 
         :param str name: Range name in A1 notation, e.g. 'A1:A5'.
         :param merge_type: (optional) one of ``MergeType.merge_all``,
             ``MergeType.merge_columns``, or ``MergeType.merge_rows``. Defaults to ``MergeType.merge_all``.
             See `MergeType`_ in the Sheets API reference.
         :type merge_type: :namedtuple:`~gspread.utils.MergeType`
@@ -2599,14 +2602,40 @@
                     },
                 },
             ]
         }
 
         return self.client.batch_update(self.spreadsheet_id, body)
 
+    def get_notes(self, default_empty_value: Optional[str] = None) -> List[List[str]]:
+        """Returns a list of lists containing all notes in the sheet, or the empty list if the
+        sheet does not have a note.
+
+        .. note::
+
+            The resulting matrix is as long as the last row holding a note
+                (could be smaller than the last data row)
+
+            The resulting matrix is as large as the last column holding a note
+                (could be smaller than the last data column)
+
+        :param str default_empty_value: (optional) Determines which value to use
+            for cells without notes, defaults to None.
+        """
+        params: ParamsType = {"fields": "sheets.data.rowData.values.note"}
+        res = self.client.spreadsheets_get(self.spreadsheet_id, params)
+        data = res["sheets"][self.index]["data"][0].get("rowData", [])
+        notes: List[List[str]] = []
+        for row in data:
+            notes.append([])
+            for cell in row.get("values", []):
+                notes[-1].append(cell.get("note", default_empty_value))
+
+        return notes
+
     def get_note(self, cell: str) -> str:
         """Get the content of the note located at `cell`, or the empty string if the
         cell does not have a note.
 
         :param str cell: A string with cell coordinates in A1 notation,
             e.g. 'D7'.
         """
@@ -3197,7 +3226,91 @@
                         "pasteType": paste_type,
                     }
                 }
             ]
         }
 
         return self.client.batch_update(self.spreadsheet_id, body)
+
+    def add_validation(
+        self,
+        range: str,
+        condition_type: ValidationConditionType,
+        values: Iterable[Any],
+        inputMessage: Optional[str] = None,
+        strict: bool = False,
+        showCustomUi: bool = False,
+    ) -> Any:
+        """Adds a data validation rule to any given range.
+
+        .. note::
+
+            ``condition_type`` values are explained here: `ConditionType`_
+
+            .. _ConditionType: https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets/other#ConditionType
+
+
+        :param str source: The A1 notation of the source range to move
+        :param condition_type: The sort of condition to apply.
+        :param values: List of condition values.
+        :type values: Any
+        :param str inputMessage: Message to show for the validation.
+        :param bool strict: Whether to reject invalid data or not.
+        :param bool showCustomUi: Whether to show a custom UI(Dropdown) for list values.
+
+        **Examples**
+
+        .. code-block:: python
+
+            import gspread
+            from gspread.utils import ValidationConditionType
+
+
+            ...
+
+            ws = spreadsheet.sheet1
+
+            ws.add_validation(
+                'A1',
+                ValidationConditionType.number_greater,
+                [10],
+                strict=True,
+                inputMessage='Value must be greater than 10',
+            )
+
+            ws.add_validation(
+                'C2:C7',
+                ValidationConditionType.one_of_list,
+                ['Yes','No'],
+                showCustomUi=True
+            )
+        """
+
+        if not isinstance(condition_type, ValidationConditionType):
+            raise TypeError(
+                "condition_type param should be a valid ValidationConditionType."
+            )
+
+        grid = a1_range_to_grid_range(range, self.id)
+
+        body = {
+            "requests": [
+                {
+                    "setDataValidation": {
+                        "range": grid,
+                        "rule": {
+                            "condition": {
+                                "type": condition_type,
+                                "values": [
+                                    ({"userEnteredValue": value}) for value in values
+                                ],
+                            },
+                            "showCustomUi": showCustomUi,
+                            "strict": strict,
+                            "inputMessage": inputMessage,
+                        },
+                    }
+                }
+            ],
+        }
+
+        return self.client.batch_update(self.spreadsheet_id, body)
```

### Comparing `gspread-6.1.0/pyproject.toml` & `gspread-6.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,15 @@
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Science/Research",
     "Topic :: Office/Business :: Financial :: Spreadsheet",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-dependencies = [
-    "google-auth>=1.12.0",
-    "google-auth-oauthlib>=0.4.1",
-    "StrEnum==0.4.15",
-]
+dependencies = ["google-auth>=1.12.0", "google-auth-oauthlib>=0.4.1"]
 requires-python = ">=3.8"
 dynamic = ["version", "description"]
 
 [project.urls]
 Documentation = "https://gspread.readthedocs.io/en/latest/"
 Source = "https://github.com/burnash/gspread"
```

### Comparing `gspread-6.1.0/PKG-INFO` & `gspread-6.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread
-Version: 6.1.0
+Version: 6.1.1
 Summary: Google Spreadsheets Python API
 Keywords: spreadsheets,google-spreadsheets,google-sheets
 Author-email: Anton Burnashev <fuss.here@gmail.com>
 Maintainer-email: Alexandre Lavigne <lavigne958@gmail.com>, alifeee <alifeee.web@outlook.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
@@ -19,15 +19,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: google-auth>=1.12.0
 Requires-Dist: google-auth-oauthlib>=0.4.1
-Requires-Dist: StrEnum==0.4.15
 Project-URL: Documentation, https://gspread.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/burnash/gspread
 
 # Google Spreadsheets Python API v4
 
 ![main workflow](https://img.shields.io/github/actions/workflow/status/burnash/gspread/main.yaml?logo=github)
 ![GitHub licence](https://img.shields.io/pypi/l/gspread?logo=github)
@@ -286,15 +285,15 @@
 cell_list = worksheet.findall(criteria_re)
 ```
 
 ### Updating Cells
 
 ```python
 # Update a single cell
-worksheet.update_acell('Bingo!', 'B1')
+worksheet.update_acell('B1', 'Bingo!')
 
 # Update a range
 worksheet.update([[1, 2], [3, 4]], 'A1:B2')
 
 # Update multiple ranges at once
 worksheet.batch_update([{
     'range': 'A1:B2',
@@ -317,14 +316,38 @@
 # Get unformatted value from the same cell range
 >>> worksheet.get("A1:B2", value_render_option=ValueRenderOption.unformatted)
 [[12]]
 
 # Get formula from a cell
 >>> worksheet.get("C2:D2", value_render_option=ValueRenderOption.formula)
 [['=1/1024']]
+### Add data validation to a range
+
+```python
+import gspread
+from gspread.utils import ValidationConditionType
+
+# Restrict the input to greater than 10 in a single cell
+worksheet.add_validation(
+  'A1',
+  ValidationConditionType.number_greater,
+  [10],
+  strict=True,
+  inputMessage='Value must be greater than 10',
+)
+
+# Restrict the input to Yes/No for a specific range with dropdown
+worksheet.add_validation(
+  'C2:C7',
+   ValidationConditionType.one_of_list,
+   ['Yes',
+   'No',]
+   showCustomUi=True
+)
+
 ```
 
 ## Documentation
 
 [Documentation]\: [https://gspread.readthedocs.io/][Documentation]
 
 [Documentation]: https://gspread.readthedocs.io/en/latest/
```

