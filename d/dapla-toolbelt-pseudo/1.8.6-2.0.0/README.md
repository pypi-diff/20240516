# Comparing `tmp/dapla_toolbelt_pseudo-1.8.6.tar.gz` & `tmp/dapla_toolbelt_pseudo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-1.8.6.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-2.0.0.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-1.8.6.tar` & `dapla_toolbelt_pseudo-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1073 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/LICENSE
--rw-r--r--   0        0        0    18202 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/README.md
--rw-r--r--   0        0        0     4728 2024-04-16 13:36:49.947715 dapla_toolbelt_pseudo-1.8.6/pyproject.toml
--rw-r--r--   0        0        0     1493 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1763 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      994 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/exceptions.py
--rw-r--r--   0        0        0      847 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      853 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0     2115 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      543 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0    12559 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/api_models.py
--rw-r--r--   0        0        0     2974 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/baseclass.py
--rw-r--r--   0        0        0     6265 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0    15341 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/depseudo.py
--rw-r--r--   0        0        0    15660 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/pseudo.py
--rw-r--r--   0        0        0     9116 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/pseudo_commons.py
--rw-r--r--   0        0        0    19278 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/repseudo.py
--rw-r--r--   0        0        0     8347 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/result.py
--rw-r--r--   0        0        0     4451 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     5611 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/validation.py
--rw-r--r--   0        0        0    19652 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-16 07:20:09.574995 dapla_toolbelt_pseudo-2.0.0/LICENSE
+-rw-r--r--   0        0        0    18193 2024-05-16 07:20:09.574995 dapla_toolbelt_pseudo-2.0.0/README.md
+-rw-r--r--   0        0        0     4936 2024-05-16 07:20:18.702990 dapla_toolbelt_pseudo-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1455 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1938 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      994 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/exceptions.py
+-rw-r--r--   0        0        0      847 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      766 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0    11244 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      555 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0    11313 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/baseclasses.py
+-rw-r--r--   0        0        0     5851 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0     8255 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/depseudo.py
+-rw-r--r--   0        0        0     2945 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/models/api.py
+-rw-r--r--   0        0        0    10591 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/models/core.py
+-rw-r--r--   0        0        0     5419 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/mutable_dataframe.py
+-rw-r--r--   0        0        0     8797 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/pseudo.py
+-rw-r--r--   0        0        0    12681 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/repseudo.py
+-rw-r--r--   0        0        0    10268 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/result.py
+-rw-r--r--   0        0        0     4451 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     5603 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/validation.py
+-rw-r--r--   0        0        0    19723 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-2.0.0/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/LICENSE` & `dapla_toolbelt_pseudo-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.6/README.md` & `dapla_toolbelt_pseudo-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
      'func': 'redact(placeholder=#)' # This is a shorthand representation of the redact function
 }
 
 rule = PseudoRule.from_json(rule_json)
 
 df = (
     Pseudonymize.from_polars(df)
-    .add_rules(rule) # Add one or more pseudonymization rules
+    .add_rules(rule) # Add to pseudonymization rules
     .run()
     .to_polars()
 )
 ```
 
 Pseudonymization rules can also be read from file. This is especially handy when there are several rules, or if you
 prefer to store and maintain pseudonymization rules externally. For example:
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/pyproject.toml` & `dapla_toolbelt_pseudo-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "1.8.6"
+version = "2.0.0"
 description = "Pseudonymization extensions for Dapla"
 authors = ["Dapla Developers <dapla-platform-developers@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
@@ -27,19 +27,23 @@
 fsspec = ">=2023.5.0"
 polars = ">=0.18.2"
 pygments = ">2.15.0"
 click = ">=8.0.1"
 ssb-datadoc-model = ">=5.0.0"
 cloudpathlib = { extras = ["gs"], version = ">=0.17.0" }
 pyarrow = ">=14.0.2, <15"
+orjson = "^3.10.1"
+wcmatch = "^8.5.1"
 
 [tool.poetry.group.test.dependencies]
 typeguard = ">=2.13.3"
 
 [tool.poetry.group.dev.dependencies]
+pytest-cases = ">=3.8.5"
+pytest-mock = ">=3.14"
 pygments = ">=2.10.0"
 black = { extras = ["jupyter"], version = ">=23.1.0" }
 coverage = { extras = ["toml"], version = ">=6.2" }
 darglint = ">=1.8.1"
 furo = ">=2021.11.12"
 mypy = ">=0.930"
 pre-commit = ">=2.16.0"
@@ -80,31 +84,39 @@
 
 [tool.mypy]
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_context = true
+disallow_untyped_decorators = false
 
 [[tool.mypy.overrides]]
 # Allow missing type hints in third-party libraries without type information.
 module = [
     "google.auth.exceptions",
     "gcsfs",
     "gcsfs.core",
     "dapla",
     "fsspec",
     "fsspec.spec",
     "typeguard",
     "puremagic",
     "google.*",
-    "google.oauth2"
+    "google.oauth2",
+    "pytest_cases",
+    "pytest_mock"
 ]
 ignore_missing_imports = true
 
+[[tool.mypy.overrides]]
+module = "dapla_pseudo.tests.*"
+disallow_untyped_defs = true
+
+
 [tool.ruff]
 force-exclude = true  # Apply excludes to pre-commit
 show-fixes = true
 src = ["src", "tests"]
 target-version = "py310"  # Minimum Python version supported
 include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
 extend-exclude = [
@@ -149,23 +161,22 @@
 convention = "google"  # You can also use "numpy".
 
 [tool.ruff.lint.pep8-naming]
 classmethod-decorators = ["classmethod", "validator", "root_validator", "pydantic.validator"]
 
 [tool.ruff.lint.per-file-ignores]
 "*/__init__.py" = ["F401"]
-"**/tests/*" = [
+"**/tests/**" = [
     # asserts are encouraged in pytest
     "S101",
     # return annotations don't add value for test functions
     "ANN201",
     # docstrings are overkill for test functions
     "D100",
     "D101",
     "D102",
     "D103",
 ]
-"tests/integration/*" = ["F401", "F811"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,25 +16,24 @@
 
 from importlib.metadata import version
 
 # Avoid having to define the version multiple places.
 # Ref: https://github.com/python-poetry/poetry/issues/144#issuecomment-1488038660
 __version__ = version("dapla_toolbelt_pseudo")
 
-from dapla_pseudo.v1.api_models import Field
-from dapla_pseudo.v1.api_models import PseudoKeyset
-from dapla_pseudo.v1.api_models import PseudoRule
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.depseudo import Depseudonymize
+from dapla_pseudo.v1.models.core import PseudoKeyset
+from dapla_pseudo.v1.models.core import PseudoRule
 from dapla_pseudo.v1.pseudo import Pseudonymize
 from dapla_pseudo.v1.repseudo import Repseudonymize
 from dapla_pseudo.v1.validation import Validator
 
 __all__ = [
     "PseudoClient",
     "Pseudonymize",
     "Depseudonymize",
     "Repseudonymize",
     "Validator",
-    "Field",
     "PseudoKeyset",
+    "PseudoRule",
 ]
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,22 @@
     PSEUDO_SERVICE_AUTH_TOKEN = "PSEUDO_SERVICE_AUTH_TOKEN"  # S105
 
     def __str__(self) -> str:
         """Use value for string representation."""
         return str(self.value)
 
 
+class PseudoOperation(str, Enum):
+    """Pseudo operation."""
+
+    PSEUDONYMIZE = "pseudonymize"
+    DEPSEUDONYMIZE = "depseudonymize"
+    REPSEUDONYMIZE = "repseudonymize"
+
+
 class PredefinedKeys(str, Enum):
     """Names of 'global keys' that the Dapla Pseudo Service is familiar with."""
 
     SSB_COMMON_KEY_1 = "ssb-common-key-1"
     SSB_COMMON_KEY_2 = "ssb-common-key-2"
     PAPIS_COMMON_KEY_1 = "papis-common-key-1"
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/exceptions.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/types.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 from pathlib import Path
 from typing import TypeAlias
 
 import fsspec
 import gcsfs
 import pandas as pd
 
-from dapla_pseudo.v1.api_models import Field
-
-FieldDecl: TypeAlias = str | dict[str, str] | Field
+FieldDecl: TypeAlias = str | dict[str, str]
 BinaryFileDecl: TypeAlias = (
     io.BufferedReader
     | fsspec.spec.AbstractBufferedFile
     | gcsfs.core.GCSFile
     | io.BytesIO
 )
 
-DatasetDecl: TypeAlias = pd.DataFrame | BinaryFileDecl | str | Path
-FileLikeDatasetDecl: TypeAlias = BinaryFileDecl | str | Path
-FileSpecDecl: TypeAlias = tuple[str | None, BinaryFileDecl | str, str]
+DatasetDecl = pd.DataFrame | BinaryFileDecl | str | Path
+FileLikeDatasetDecl = BinaryFileDecl | str | Path
+FileSpecDecl = tuple[str | None, BinaryFileDecl | str, str]
 # FileSpecDecl is derived from the "files" argument in multi-part requests from the "Requests"-library
 # The tuple semantically means: ('filename', fileobj, 'content_type')
 # See "files" in https://requests.readthedocs.io/en/latest/api/#requests.request
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/__init__.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Pseudo Service version 1 implementation."""
 
-from dapla_pseudo.v1.api_models import Field
-from dapla_pseudo.v1.api_models import PseudoKeyset
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.depseudo import Depseudonymize
+from dapla_pseudo.v1.models.core import PseudoKeyset
+from dapla_pseudo.v1.models.core import PseudoRule
 from dapla_pseudo.v1.pseudo import Pseudonymize
 from dapla_pseudo.v1.repseudo import Repseudonymize
 from dapla_pseudo.v1.validation import Validator
 
 __all__ = [
     "PseudoClient",
     "Pseudonymize",
     "Depseudonymize",
     "Repseudonymize",
     "Validator",
-    "Field",
     "PseudoKeyset",
+    "PseudoRule",
 ]
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/api_models.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/models/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,48 @@
-"""This module defines helper classes and API models used to communicate with the Dapla Pseudo Service."""
-
 import json
 import typing as t
+from dataclasses import dataclass
 from datetime import date
 from enum import Enum
 
 from humps import camelize
 from pydantic import BaseModel
 from pydantic import ConfigDict
+from pydantic import Field
 from pydantic import FieldSerializationInfo
 from pydantic import ValidationError
 from pydantic import field_serializer
 from pydantic import model_serializer
 from pydantic import model_validator
 
 from dapla_pseudo.constants import MapFailureStrategy
 from dapla_pseudo.constants import PredefinedKeys
 from dapla_pseudo.constants import PseudoFunctionTypes
 from dapla_pseudo.constants import UnknownCharacterStrategy
 from dapla_pseudo.models import APIModel
+from dapla_pseudo.types import BinaryFileDecl
 
 
 class Mimetypes(str, Enum):
     """Mimetypes is an enum of supported mimetypes, for use in HTTP requests.
 
     As a proxy, this also defines the supported input file formats when reading from a file.
     """
 
     JSON = "application/json"
     ZIP = "application/zip"
     CSV = "text/csv"
 
 
-class Field(APIModel):
-    """Field represents a targeted piece of data within a dataset or record.
-
-    Parameters:
-        pattern: field name or expression (e.g. a glob)
-        mapping: If defined, denotes a mapping transformation that should be applied before the operation in question,
-            e.g. "sid", meaning the field should be transformed to Stabil ID before being pseudonymized.
-    """
-
-    pattern: str
-    mapping: str | None = None
-
-
-class PseudoKeyset(APIModel):
-    """PseudoKeyset represents a wrapped data encryption key (WDEK).
-
-    Example structure, represented as JSON:
-    {"encrypted_keyset": "CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",
-    "keyset_info": {
-    "primaryKeyId": 1234567890,
-    "keyInfo": [
-    {
-    "typeUrl": "type.googleapis.com/google.crypto.tink.AesSivKey",
-    "status": "ENABLED",
-    "keyId": 1234567890,
-    "outputPrefixType": "TINK"
-    }
-    ]
-    },
-    "kek_uri": "gcp-kms://projects/some-project-id/locations/europe-north1/keyRings/some-keyring/cryptoKeys/some-kek-1"
-    }
-    """
-
-    encrypted_keyset: str
-    keyset_info: dict[str, t.Any]
-    kek_uri: str
-
-    def get_key_id(self) -> str:
-        """ID of the keyset."""
-        return str(self.keyset_info["primaryKeyId"])
-
-
-class TargetCompression(APIModel):
-    """TargetCompression denotes if and how results from the API should be compressed and password encrypted."""
-
-    password: str
-
-
-class KeyWrapper(BaseModel):
-    """Hold information about a key, such as ID and keyset information."""
-
-    key_id: str = ""
-    keyset: PseudoKeyset | None = None
-
-    def __init__(self, key: str | PseudoKeyset | None = None, **kwargs: t.Any) -> None:
-        """Determine if a key is either a key reference (aka "common key") or a keyset.
-
-        If it is a key reference, treat this as the key's ID, else retrieve the key's ID from the keyset data structure.
-
-        :param key: either a key reference (as string) or a PseudoKeyset
-        """
-        super().__init__(**kwargs)
-        if isinstance(key, str):
-            try:  # Attempt to parse the key as a JSON-string matching the PseudoKeyset model
-                pseudo_keyset = PseudoKeyset.model_validate(json.loads(key))
-                self.key_id = pseudo_keyset.get_key_id()
-                self.keyset = pseudo_keyset
-                return
-            except (ValidationError, json.JSONDecodeError):
-                pass
-
-            # Else, attempt to parse the key as one of the predefined keys
-            if key in PredefinedKeys.__members__.values():
-                self.key_id = key
-                self.keyset = None
-            else:
-                raise ValueError(f"Key '{key}' is not a valid key reference or keyset")
-        # Or we have an already parsed PseudoKeyset
-        elif isinstance(key, PseudoKeyset):
-            self.key_id = key.get_key_id()
-            self.keyset = key
+@dataclass
+class File:
+    """'File' represents a file to be pseudonymized."""
 
-    def keyset_list(self) -> list[PseudoKeyset] | None:
-        """Wrap the keyset in a list if it is defined - or return None if it is not."""
-        return None if self.keyset is None else [self.keyset]
+    file_handle: BinaryFileDecl
+    content_type: Mimetypes
 
 
 class PseudoFunctionArgs(BaseModel):
     """Representation of the possible keyword arguments."""
 
     def __str__(self) -> str:
         """As a default, represent the fields of the subclasses as kwargs on the format 'k=v'."""
@@ -141,15 +63,15 @@
         snapshot_date (date): The timestamp for the version of the SID catalogue.
             If not specified, will choose the latest version.
             The format is: YYYY-MM-DD, e.g. 2021-05-21
         strategy: defines how encryption/decryption should handle non-alphabet characters
         failure_strategy: defines how to handle mapping failures
     """
 
-    key_id: PredefinedKeys | str = PredefinedKeys.PAPIS_COMMON_KEY_1
+    key_id: PredefinedKeys | str = Field(default=PredefinedKeys.PAPIS_COMMON_KEY_1)
     snapshot_date: date | None = None
     strategy: UnknownCharacterStrategy | None = UnknownCharacterStrategy.SKIP
     failure_strategy: MapFailureStrategy | None = None
 
 
 class DaeadKeywordArgs(PseudoFunctionArgs):
     """Representation of kwargs for the 'daead' function."""
@@ -284,69 +206,86 @@
         """Deserialise the json-formatted pseudo rule to Python model."""
         if isinstance(data, str):
             return super().model_validate(json.loads(data))
         else:
             return super().model_validate(data)
 
 
-class PseudoFieldRequest(APIModel):
-    """Model of the pseudo field request sent to the service."""
-
-    pseudo_func: PseudoFunction
-    name: str
-    values: list[str]
-    keyset: PseudoKeyset | None = None
-
-
-class DepseudoFieldRequest(APIModel):
-    """Model of the depseudo field request sent to the service."""
-
-    pseudo_func: PseudoFunction
-    name: str
-    values: list[str]
-    keyset: PseudoKeyset | None = None
+class PseudoKeyset(APIModel):
+    """PseudoKeyset represents a wrapped data encryption key (WDEK).
 
+    Example structure, represented as JSON:
+    {"encrypted_keyset": "CiQAp91NBhLdknX3j9jF6vwhdyURaqcT9/M/iczV7fLn...8XYFKwxiwMtCzDT6QGzCCCM=",
+    "keyset_info": {
+    "primaryKeyId": 1234567890,
+    "keyInfo": [
+    {
+    "typeUrl": "type.googleapis.com/google.crypto.tink.AesSivKey",
+    "status": "ENABLED",
+    "keyId": 1234567890,
+    "outputPrefixType": "TINK"
+    }
+    ]
+    },
+    "kek_uri": "gcp-kms://projects/some-project-id/locations/europe-north1/keyRings/some-keyring/cryptoKeys/some-kek-1"
+    }
+    """
 
-class RepseudoFieldRequest(APIModel):
-    """Model of the repseudo field request sent to the service."""
+    encrypted_keyset: str
+    keyset_info: dict[str, t.Any]
+    kek_uri: str
 
-    source_pseudo_func: PseudoFunction
-    target_pseudo_func: PseudoFunction
-    name: str
-    values: list[str]
-    source_keyset: PseudoKeyset | None = None
-    target_keyset: PseudoKeyset | None = None
+    def get_key_id(self) -> str:
+        """ID of the keyset."""
+        return str(self.keyset_info["primaryKeyId"])
 
 
 class PseudoConfig(APIModel):
     """PseudoConfig is a container for rules and keysets."""
 
     rules: list[PseudoRule]
     keysets: list[PseudoKeyset] | None = None
 
 
-class PseudonymizeFileRequest(APIModel):
-    """PseudonymizeFileRequest represents a request towards pseudonymize file API endpoints."""
+class TargetCompression(APIModel):
+    """TargetCompression denotes if and how results from the API should be compressed and password encrypted."""
 
-    pseudo_config: PseudoConfig
-    target_uri: str | None = None
-    target_content_type: Mimetypes
-    compression: TargetCompression | None = None
+    password: str
 
 
-class DepseudonymizeFileRequest(APIModel):
-    """DepseudonymizeFileRequest represents a request towards depseudonymize file API endpoints."""
+class KeyWrapper(BaseModel):
+    """Hold information about a key, such as ID and keyset information."""
+
+    key_id: str = ""
+    keyset: PseudoKeyset | None = None
+
+    def __init__(self, key: str | PseudoKeyset | None = None, **kwargs: t.Any) -> None:
+        """Determine if a key is either a key reference (aka "common key") or a keyset.
 
-    pseudo_config: PseudoConfig
-    target_uri: str | None = None
-    target_content_type: Mimetypes
-    compression: TargetCompression | None = None
+        If it is a key reference, treat this as the key's ID, else retrieve the key's ID from the keyset data structure.
 
+        :param key: either a key reference (as string) or a PseudoKeyset
+        """
+        super().__init__(**kwargs)
+        if isinstance(key, str):
+            try:  # Attempt to parse the key as a JSON-string matching the PseudoKeyset model
+                pseudo_keyset = PseudoKeyset.model_validate(json.loads(key))
+                self.key_id = pseudo_keyset.get_key_id()
+                self.keyset = pseudo_keyset
+                return
+            except (ValidationError, json.JSONDecodeError):
+                pass
 
-class RepseudonymizeFileRequest(APIModel):
-    """RepseudonymizeFileRequest represents a request towards repseudonymize file API endpoints."""
+            # Else, attempt to parse the key as one of the predefined keys
+            if key in PredefinedKeys.__members__.values():
+                self.key_id = key
+                self.keyset = None
+            else:
+                raise ValueError(f"Key '{key}' is not a valid key reference or keyset")
+        # Or we have an already parsed PseudoKeyset
+        elif isinstance(key, PseudoKeyset):
+            self.key_id = key.get_key_id()
+            self.keyset = key
 
-    source_pseudo_config: PseudoConfig
-    target_pseudo_config: PseudoConfig
-    target_uri: str | None = None
-    target_content_type: Mimetypes
-    compression: TargetCompression | None = None
+    def keyset_list(self) -> list[PseudoKeyset] | None:
+        """Wrap the keyset in a list if it is defined - or return None if it is not."""
+        return None if self.keyset is None else [self.keyset]
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,32 +9,23 @@
 import requests
 from dapla import AuthClient
 from ulid import ULID
 
 from dapla_pseudo.constants import TIMEOUT_DEFAULT
 from dapla_pseudo.constants import Env
 from dapla_pseudo.types import FileSpecDecl
-from dapla_pseudo.v1.api_models import DepseudoFieldRequest
-from dapla_pseudo.v1.api_models import DepseudonymizeFileRequest
-from dapla_pseudo.v1.api_models import Mimetypes
-from dapla_pseudo.v1.api_models import PseudoFieldRequest
-from dapla_pseudo.v1.api_models import PseudonymizeFileRequest
-from dapla_pseudo.v1.api_models import RepseudoFieldRequest
-from dapla_pseudo.v1.api_models import RepseudonymizeFileRequest
+from dapla_pseudo.v1.models.api import DepseudoFieldRequest
+from dapla_pseudo.v1.models.api import PseudoFieldRequest
+from dapla_pseudo.v1.models.api import RepseudoFieldRequest
+from dapla_pseudo.v1.models.core import Mimetypes
 
 
 class PseudoClient:
     """Client for interacting with the Dapla Pseudo Service REST API."""
 
-    pseudo_op_to_endpoint: t.ClassVar[dict[type, str]] = {
-        PseudonymizeFileRequest: "pseudonymize/file",
-        DepseudonymizeFileRequest: "depseudonymize/file",
-        RepseudonymizeFileRequest: "repseudonymize/file",
-    }
-
     def __init__(
         self,
         pseudo_service_url: str | None = None,
         auth_token: str | None = None,
     ) -> None:
         """Use a default url for dapla-pseudo-service if not explicitly set."""
         self.pseudo_service_url = (
@@ -77,14 +68,15 @@
 
     def _post_to_file_endpoint(
         self,
         path: str,
         request_spec: FileSpecDecl,
         data_spec: FileSpecDecl,
         stream: bool,
+        timeout: int,
     ) -> requests.Response:
         """POST to a file endpoint in the Pseudo Service.
 
         Requests to the file endpoint are sent as multi-part requests,
         where the first part represents the filedata itself, and the second part represents
         the transformations to apply on that data.
         """
@@ -93,15 +85,15 @@
             headers={
                 "Authorization": f"Bearer {self.__auth_token()}",
                 "Accept-Encoding": "gzip",
                 "X-Correlation-Id": PseudoClient._generate_new_correlation_id(),
             },
             files={"data": data_spec, "request": request_spec},
             stream=stream,
-            timeout=TIMEOUT_DEFAULT,
+            timeout=timeout,
         )
 
         PseudoClient._handle_response_error(response)
         return response
 
     def _post_to_field_endpoint(
         self,
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/depseudo.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/repseudo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,342 +1,268 @@
 """Builder for submitting a pseudonymization request."""
 
-import os
 import typing as t
-from concurrent.futures import ThreadPoolExecutor
-from concurrent.futures import as_completed
 from datetime import date
 
 import pandas as pd
 import polars as pl
 
 from dapla_pseudo.constants import TIMEOUT_DEFAULT
-from dapla_pseudo.constants import Env
-from dapla_pseudo.constants import MapFailureStrategy
 from dapla_pseudo.constants import PredefinedKeys
-from dapla_pseudo.constants import PseudoFunctionTypes
+from dapla_pseudo.constants import PseudoOperation
 from dapla_pseudo.types import FileLikeDatasetDecl
-from dapla_pseudo.utils import convert_to_date
-from dapla_pseudo.v1.api_models import DaeadKeywordArgs
-from dapla_pseudo.v1.api_models import DepseudoFieldRequest
-from dapla_pseudo.v1.api_models import DepseudonymizeFileRequest
-from dapla_pseudo.v1.api_models import FF31KeywordArgs
-from dapla_pseudo.v1.api_models import KeyWrapper
-from dapla_pseudo.v1.api_models import MapSidKeywordArgs
-from dapla_pseudo.v1.api_models import Mimetypes
-from dapla_pseudo.v1.api_models import PseudoConfig
-from dapla_pseudo.v1.api_models import PseudoFunction
-from dapla_pseudo.v1.api_models import PseudoKeyset
-from dapla_pseudo.v1.api_models import PseudoRule
-from dapla_pseudo.v1.client import PseudoClient
-from dapla_pseudo.v1.pseudo_commons import File
-from dapla_pseudo.v1.pseudo_commons import PseudoFieldResponse
-from dapla_pseudo.v1.pseudo_commons import PseudoFileResponse
-from dapla_pseudo.v1.pseudo_commons import RawPseudoMetadata
-from dapla_pseudo.v1.pseudo_commons import get_file_data_from_dataset
-from dapla_pseudo.v1.pseudo_commons import pseudo_operation_dataset
-from dapla_pseudo.v1.pseudo_commons import pseudonymize_operation_field
+from dapla_pseudo.utils import get_file_data_from_dataset
+from dapla_pseudo.v1.baseclasses import _BasePseudonymizer
+from dapla_pseudo.v1.baseclasses import _BaseRuleConstructor
+from dapla_pseudo.v1.models.core import File
+from dapla_pseudo.v1.models.core import PseudoFunction
+from dapla_pseudo.v1.models.core import PseudoKeyset
+from dapla_pseudo.v1.models.core import PseudoRule
 from dapla_pseudo.v1.result import Result
 
 
-class Depseudonymize:
-    """Starting point for depseudonymization of datasets.
+class Repseudonymize:
+    """Starting point for pseudonymization of datasets.
 
     This class should not be instantiated, only the static methods should be used.
     """
 
     dataset: File | pl.DataFrame
 
     @staticmethod
-    def from_pandas(dataframe: pd.DataFrame) -> "Depseudonymize._Depseudonymizer":
-        """Initialize a depseudonymization request from a pandas DataFrame."""
+    def from_pandas(
+        dataframe: pd.DataFrame, run_as_file: bool = False
+    ) -> "Repseudonymize._Repseudonymizer":
+        """Initialize a pseudonymization request from a pandas DataFrame."""
         dataset: pl.DataFrame = pl.from_pandas(dataframe)
-        Depseudonymize.dataset = dataset
-        return Depseudonymize._Depseudonymizer()
+        if run_as_file:
+            file_handle, content_type = get_file_data_from_dataset(dataset)
+            Repseudonymize.dataset = File(file_handle, content_type)
+        else:
+            Repseudonymize.dataset = dataset
+        return Repseudonymize._Repseudonymizer()
 
     @staticmethod
-    def from_polars(dataframe: pl.DataFrame) -> "Depseudonymize._Depseudonymizer":
-        """Initialize a depseudonymization request from a polars DataFrame."""
-        Depseudonymize.dataset = dataframe
-        return Depseudonymize._Depseudonymizer()
+    def from_polars(
+        dataframe: pl.DataFrame, run_as_file: bool = False
+    ) -> "Repseudonymize._Repseudonymizer":
+        """Initialize a pseudonymization request from a polars DataFrame."""
+        if run_as_file:
+            file_handle, content_type = get_file_data_from_dataset(dataframe)
+            Repseudonymize.dataset = File(file_handle, content_type)
+        else:
+            Repseudonymize.dataset = dataframe
+        return Repseudonymize._Repseudonymizer()
 
     @staticmethod
-    def from_file(dataset: FileLikeDatasetDecl) -> "Depseudonymize._Depseudonymizer":
-        """Initialize a depseudonymization request from a pandas dataframe read from file.
+    def from_file(dataset: FileLikeDatasetDecl) -> "Repseudonymize._Repseudonymizer":
+        """Initialize a pseudonymization request from a pandas dataframe read from file.
 
         Args:
             dataset (FileLikeDatasetDecl): Either a path to the file to be read, or a file handle.
 
         Returns:
-            _Depseudonymizer: An instance of the _Depseudonymizer class.
+            _Pseudonymizer: An instance of the _Pseudonymizer class.
 
         Examples:
             # Read from bucket
             from dapla import AuthClient
-            from dapla_pseudo import Depseudonymize
+            from dapla_pseudo import Pseudonymize
             bucket_path = "gs://ssb-staging-dapla-felles-data-delt/felles/smoke-tests/fruits/data.parquet"
-            field_selector = Depseudonymize.from_file(bucket_path)
+            field_selector = Pseudonymize.from_file(bucket_path)
 
             # Read from local filesystem
-            from dapla_pseudo import Depseudonymize
+            from dapla_pseudo import Pseudonymize
 
             local_path = "some_file.csv"
-            field_selector = Depseudonymize.from_file(local_path))
+            field_selector = Pseudonymize.from_file(local_path))
         """
         file_handle, content_type = get_file_data_from_dataset(dataset)
-        Depseudonymize.dataset = File(file_handle, content_type)
-        return Depseudonymize._Depseudonymizer()
+        Repseudonymize.dataset = File(file_handle, content_type)
+        return Repseudonymize._Repseudonymizer()
 
-    class _Depseudonymizer:
+    class _Repseudonymizer(_BasePseudonymizer):
         """Select one or multiple fields to be pseudonymized."""
 
-        def __init__(self, rules: list[PseudoRule] | None = None) -> None:
+        source_rules: t.ClassVar[list[PseudoRule]] = []
+        target_rules: t.ClassVar[list[PseudoRule]] = []
+
+        def __init__(
+            self,
+            source_rules: list[PseudoRule] | None = None,
+            target_rules: list[PseudoRule] | None = None,
+        ) -> None:
             """Initialize the class."""
-            self._rules: list[PseudoRule] = [] if rules is None else rules
-            self._pseudo_keyset: PseudoKeyset | str | None = None
-            self._timeout: int = TIMEOUT_DEFAULT
-            self._pseudo_client: PseudoClient = PseudoClient(
-                pseudo_service_url=os.getenv(Env.PSEUDO_SERVICE_URL),
-                auth_token=os.getenv(Env.PSEUDO_SERVICE_AUTH_TOKEN),
+            if source_rules is None or target_rules is None:
+                # Because the "source_rules" and "target_rules" are static class variables,
+                # we need to reset the lists when the first call to "_Repseudonymizer" is made.
+                # This is because if we were to use the base class "Repseudonymize" twice in the same file,
+                # the lists of rules would persist across runs.
+                # *This is very hacky*, but the alternative is to pass the rules through
+                # "_RepseudoFuncSelectorSource" and "_RepseudoFuncSelectorTarget", which would hurt readability
+                Repseudonymize._Repseudonymizer.source_rules = []
+                Repseudonymize._Repseudonymizer.target_rules = []
+            else:
+                Repseudonymize._Repseudonymizer.source_rules.extend(source_rules)
+                Repseudonymize._Repseudonymizer.target_rules.extend(target_rules)
+
+            super().__init__(
+                pseudo_operation=PseudoOperation.REPSEUDONYMIZE,
+                dataset=Repseudonymize.dataset,
             )
 
-        def on_fields(self, *fields: str) -> "Depseudonymize._DepseudoFuncSelector":
-            """Specify one or multiple fields to be depseudonymized."""
-            return Depseudonymize._DepseudoFuncSelector(list(fields), self._rules)
+        def on_fields(
+            self, *fields: str
+        ) -> "Repseudonymize._RepseudoFuncSelectorSource":
+            """Specify one or multiple fields to be pseudonymized."""
+            return Repseudonymize._RepseudoFuncSelectorSource(list(fields))
 
         def run(
             self,
-            custom_keyset: PseudoKeyset | str | None = None,
+            source_custom_keyset: PseudoKeyset | str | None = None,
+            target_custom_keyset: PseudoKeyset | str | None = None,
             timeout: int = TIMEOUT_DEFAULT,
         ) -> Result:
-            """Depseudonymize the dataset.
+            """Pseudonymize the dataset.
 
             Args:
-                custom_keyset (PseudoKeyset | str, optional): The depseudonymization keyset to use.
-                    This can either be a PseudoKeyset, a JSON-string matching the fields of PseudoKeyset,
-                    or a string matching one of the keys in `dapla_pseudo.constants.PredefinedKeys`. the Defaults to None.
+                source_custom_keyset (PseudoKeyset, optional): The source pseudonymization keyset to use. Defaults to None.
+                target_custom_keyset (PseudoKeyset, optional): The target pseudonymization keyset to use. Defaults to None.
                 timeout (int): The timeout in seconds for the API call. Defaults to TIMEOUT_DEFAULT.
 
-            Raises:
-                ValueError: If no dataset has been provided, no fields have been provided, or the dataset is of an unsupported type.
-
             Returns:
-                Result: The depseudonymized dataset and the associated metadata.
+                Result: The pseudonymized dataset and the associated metadata.
             """
-            if Depseudonymize.dataset is None:
-                raise ValueError("No dataset has been provided.")
-
-            if self._rules == []:
-                raise ValueError(
-                    "No fields have been provided. Use the 'on_fields' method."
-                )
-
-            if custom_keyset is not None:
-                self._pseudo_keyset = custom_keyset
-
-            self._timeout = timeout
-            match Depseudonymize.dataset:  # Differentiate between file and DataFrame
-                case File():
-                    return self._depseudonymize_file()
-                case pl.DataFrame():
-                    return self._depseudonymize_field()
-                case _ as invalid_dataset:
-                    raise ValueError(
-                        f"Unsupported data type: {type(invalid_dataset)}. Should only be DataFrame or file-like type."
-                    )
-
-        def _depseudonymize_file(self) -> Result:
-            """Depseudonymize the entire file."""
-            # Need to type-cast explicitly. We know that Depseudonymize.dataset is a "File" if we reach this method.
-            file = t.cast(File, Depseudonymize.dataset)
-
-            depseudonymize_request = DepseudonymizeFileRequest(
-                pseudo_config=PseudoConfig(
-                    rules=self._rules,
-                    keysets=KeyWrapper(self._pseudo_keyset).keyset_list(),
-                ),
-                target_content_type=Mimetypes.JSON,
-                target_uri=None,
-                compression=None,
+            return super()._execute_pseudo_operation(
+                rules=self.source_rules,
+                target_rules=self.target_rules,
+                custom_keyset=source_custom_keyset,
+                target_custom_keyset=target_custom_keyset,
+                timeout=timeout,
             )
 
-            pseudo_response: PseudoFileResponse = pseudo_operation_dataset(
-                dataset_ref=file,
-                pseudo_operation_request=depseudonymize_request,
+    class _RepseudoFuncSelectorSource(_BaseRuleConstructor):
+        def __init__(self, fields: list[str]) -> None:
+            self.fields = fields
+            super().__init__(fields, type(Repseudonymize.dataset))
+
+        def from_stable_id(
+            self,
+            sid_snapshot_date: str | date | None = None,
+            custom_key: PredefinedKeys | str | None = None,
+        ) -> "Repseudonymize._RepseudoFuncSelectorTarget":
+            """Claim that the selected fields were mapped to Stable ID, then pseudonymized with PAPIS-compatible encryption.
+
+            Args:
+                sid_snapshot_date (Optional[str | date], optional): Date representing SID-catalogue version that was used.
+                    Latest if unspecified. Format: YYYY-MM-DD
+                custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
+                    Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
+
+            Returns:
+                An object with methods to choose how the field should be pseudonymized.
+            """
+            rules = super()._map_to_stable_id_and_pseudonymize(
+                sid_snapshot_date, custom_key
             )
-            return Result(pseudo_response=pseudo_response)
+            return Repseudonymize._RepseudoFuncSelectorTarget(self.fields, rules)
 
-        def _depseudonymize_field(self) -> Result:
-            """Depseudonymizes the specified fields in the DataFrame using the provided pseudonymization function.
+        def from_default_encryption(
+            self, custom_key: PredefinedKeys | str | None = None
+        ) -> "Repseudonymize._RepseudoFuncSelectorTarget":
+            """Claim that the selected fields were pseudonymized with default encryption.
 
-            The depseudonymization is performed in parallel. After the parallel processing is finished,
-            the depseudonymized fields replace the original fields in the DataFrame stored in `self._dataframe`.
+            Args:
+                custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
+                    Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
 
             Returns:
-                Result: Containing the depseudonymized 'self._dataframe' and the associated metadata.
+                An object with methods to choose how the field should be pseudonymized.
             """
+            rules = super()._with_daead_encryption(custom_key)
+            return Repseudonymize._RepseudoFuncSelectorTarget(self.fields, rules)
 
-            def depseudonymize_field_runner(
-                field_name: str, series: pl.Series, pseudo_func: PseudoFunction
-            ) -> tuple[str, pl.Series, RawPseudoMetadata]:
-                """Function that performs the pseudonymization on a pandas Series.
-
-                Args:
-                    field_name (str):  The name of the field.
-                    series (pl.Series): The pandas Series containing the values to be pseudonymized.
-                    pseudo_func (PseudoFunction): The pseudonymization function to apply to the values.
-
-                Returns:
-                    tuple[str,pl.Series]: A tuple containing the field_name and the corresponding series.
-                """
-                request = DepseudoFieldRequest(
-                    pseudo_func=pseudo_func,
-                    keyset=KeyWrapper(self._pseudo_keyset).keyset,
-                    name=field_name,
-                    values=series.to_list(),
-                )
-                data, metadata = pseudonymize_operation_field(
-                    path="depseudonymize/field",
-                    pseudo_field_request=request,
-                    timeout=self._timeout,
-                    pseudo_client=self._pseudo_client,
-                )
-                return field_name, data, metadata
-
-            dataframe = t.cast(pl.DataFrame, Depseudonymize.dataset)
-            # Execute the pseudonymization API calls in parallel
-            with ThreadPoolExecutor() as executor:
-                depseudonymized_field: dict[str, pl.Series] = {}
-                raw_metadata_fields: list[RawPseudoMetadata] = []
-                futures = [
-                    executor.submit(
-                        depseudonymize_field_runner,
-                        rule.pattern,
-                        dataframe[rule.pattern],
-                        rule.func,
-                    )
-                    for rule in self._rules
-                ]
-                # Wait for the futures to finish, then add each field to pseudonymized_field map
-                for future in as_completed(futures):
-                    field_name, data, raw_metadata = future.result()
-                    depseudonymized_field[field_name] = data
-                    raw_metadata_fields.append(raw_metadata)
-
-                depseudonymized_df = pl.DataFrame(depseudonymized_field)
-                dataframe = dataframe.update(depseudonymized_df)
-            return Result(
-                pseudo_response=PseudoFieldResponse(
-                    data=dataframe, raw_metadata=raw_metadata_fields
-                )
-            )
+        def from_papis_compatible_encryption(
+            self, custom_key: PredefinedKeys | str | None = None
+        ) -> "Repseudonymize._RepseudoFuncSelectorTarget":
+            """Claim that the selected fields were pseudonymized with PAPIS-compatible encryption.
 
-    class _DepseudoFuncSelector:
-        def __init__(
-            self, fields: list[str], rules: list[PseudoRule] | None = None
-        ) -> None:
-            self._fields = fields
-            self._existing_rules = [] if rules is None else rules
+            Args:
+                custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
+                    Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
+
+            Returns:
+                An object with methods to choose how the field should be pseudonymized.
+            """
+            rules = super()._with_ff31_encryption(custom_key)
+            return Repseudonymize._RepseudoFuncSelectorTarget(self.fields, rules)
+
+        def from_custom_function(
+            self, function: PseudoFunction
+        ) -> "Repseudonymize._RepseudoFuncSelectorTarget":
+            """Claim that the selected fields were pseudonymized with a custom, specified Pseudo Function."""
+            rules = super()._with_custom_function(function)
+            return Repseudonymize._RepseudoFuncSelectorTarget(self.fields, rules)
+
+    class _RepseudoFuncSelectorTarget(_BaseRuleConstructor):
+        def __init__(self, fields: list[str], source_rules: list[PseudoRule]) -> None:
+            self.source_rules = source_rules
+            super().__init__(fields, type(Repseudonymize.dataset))
 
-        def with_stable_id(
+        def to_stable_id(
             self,
             sid_snapshot_date: str | date | None = None,
-            custom_key: str | None = None,
-            on_map_failure: MapFailureStrategy | str | None = None,
-        ) -> "Depseudonymize._Depseudonymizer":
-            """Depseudonymize the selected fields with the default encryption algorithm (DAEAD).
+            custom_key: PredefinedKeys | str | None = None,
+        ) -> "Repseudonymize._Repseudonymizer":
+            """Map the selected fields to Stable ID, then pseudonymize with a PAPIS-compatible encryption.
 
-            1) Decrypt stable-id
-            2) Then map decrypted stable-id to fnr and return original fnr.
+            In other words, this is a compound operation that both: 1) maps FNR to stable ID 2) then encrypts the Stable IDs.
 
             Args:
                 sid_snapshot_date (Optional[str | date], optional): Date representing SID-catalogue version to use.
                     Latest if unspecified. Format: YYYY-MM-DD
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
-                on_map_failure (Optional[MapFailureStrategy], optional): defines how to handle mapping failures
 
             Returns:
-                Self: The object configured to be mapped to fnr
+                Self: The object configured to be mapped to stable ID
             """
-            kwargs = (
-                MapSidKeywordArgs(
-                    key_id=custom_key,
-                    snapshot_date=convert_to_date(sid_snapshot_date),
-                    failure_strategy=(
-                        None
-                        if on_map_failure is None
-                        else MapFailureStrategy(on_map_failure)
-                    ),
-                )
-                if custom_key
-                else MapSidKeywordArgs(
-                    snapshot_date=convert_to_date(sid_snapshot_date),
-                    failure_strategy=(
-                        None
-                        if on_map_failure is None
-                        else MapFailureStrategy(on_map_failure)
-                    ),
-                )
-            )
-            function = PseudoFunction(
-                function_type=PseudoFunctionTypes.MAP_SID, kwargs=kwargs
+            rules = super()._map_to_stable_id_and_pseudonymize(
+                sid_snapshot_date, custom_key
             )
-            return self._rule_constructor(function)
+            return Repseudonymize._Repseudonymizer(self.source_rules, rules)
 
-        def with_default_encryption(
+        def to_default_encryption(
             self, custom_key: PredefinedKeys | str | None = None
-        ) -> "Depseudonymize._Depseudonymizer":
-            """Depseudonymize the selected fields with the default encryption algorithm (DAEAD).
+        ) -> "Repseudonymize._Repseudonymizer":
+            """Pseudonymize the selected fields with the default encryption algorithm (DAEAD).
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (ssb-common-key-1)
 
             Returns:
                 Self: The object configured to be mapped to stable ID
             """
-            kwargs = (
-                DaeadKeywordArgs(key_id=custom_key)
-                if custom_key
-                else DaeadKeywordArgs()
-            )
-            function = PseudoFunction(
-                function_type=PseudoFunctionTypes.DAEAD, kwargs=kwargs
-            )
-            return self._rule_constructor(function)
+            rules = super()._with_daead_encryption(custom_key)
+            return Repseudonymize._Repseudonymizer(self.source_rules, rules)
 
-        def with_papis_compatible_encryption(
+        def to_papis_compatible_encryption(
             self, custom_key: PredefinedKeys | str | None = None
-        ) -> "Depseudonymize._Depseudonymizer":
-            """Depseudonymize the selected fields with a PAPIS-compatible encryption algorithm (FF31).
+        ) -> "Repseudonymize._Repseudonymizer":
+            """Pseudonymize the selected fields with a PAPIS-compatible encryption algorithm (FF31).
 
             Args:
                 custom_key (Optional[PredefinedKeys | str], optional): Override the key to use for pseudonymization.
                     Must be one of the keys defined in PredefinedKeys. If not defined, uses the default key for this function (papis-common-key-1)
 
             Returns:
                 Self: The object configured to be mapped to stable ID
             """
-            kwargs = (
-                FF31KeywordArgs(key_id=custom_key) if custom_key else FF31KeywordArgs()
-            )
-            function = PseudoFunction(
-                function_type=PseudoFunctionTypes.FF31, kwargs=kwargs
-            )
-            return self._rule_constructor(function)
+            rules = super()._with_ff31_encryption(custom_key)
+            return Repseudonymize._Repseudonymizer(self.source_rules, rules)
 
-        def with_custom_function(
+        def to_custom_function(
             self, function: PseudoFunction
-        ) -> "Depseudonymize._Depseudonymizer":
-            return self._rule_constructor(function)
-
-        def _rule_constructor(
-            self, func: PseudoFunction
-        ) -> "Depseudonymize._Depseudonymizer":
-            # If we use the depseudonymize_file endpoint, we need a glob catch-all prefix.
-            rule_prefix = "**/" if isinstance(Depseudonymize.dataset, File) else ""
-            rules = [
-                PseudoRule(name=None, func=func, pattern=f"{rule_prefix}{field}")
-                for field in self._fields
-            ]
-            return Depseudonymize._Depseudonymizer(self._existing_rules + rules)
+        ) -> "Repseudonymize._Repseudonymizer":
+            rules = super()._with_custom_function(function)
+            return Repseudonymize._Repseudonymizer(self.source_rules, rules)
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/result.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/result.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,64 @@
 """Common API models for builder packages."""
 
-import typing as t
+from collections import Counter
 from io import BufferedWriter
 from pathlib import Path
 from typing import Any
+from typing import cast
 
 import pandas as pd
 import polars as pl
 from cloudpathlib import GSClient
 from cloudpathlib import GSPath
 from dapla import AuthClient
 from datadoc_model.model import MetadataContainer
 from datadoc_model.model import PseudonymizationMetadata
 from datadoc_model.model import PseudoVariable
 
 from dapla_pseudo.utils import get_file_format_from_file_name
-from dapla_pseudo.v1.pseudo_commons import PseudoFieldResponse
-from dapla_pseudo.v1.pseudo_commons import PseudoFileResponse
+from dapla_pseudo.v1.models.api import PseudoFieldResponse
+from dapla_pseudo.v1.models.api import PseudoFileResponse
 from dapla_pseudo.v1.supported_file_format import SupportedOutputFileFormat
 from dapla_pseudo.v1.supported_file_format import write_from_df
 from dapla_pseudo.v1.supported_file_format import write_from_dicts
 
 
 class Result:
     """Result represents the result of a pseudonymization operation."""
 
     def __init__(
         self,
         pseudo_response: PseudoFieldResponse | PseudoFileResponse,
     ) -> None:
         """Initialise a PseudonymizationResult."""
-        self._pseudo_data: pl.DataFrame | list[dict[str, t.Any]]
+        self._pseudo_data: pl.DataFrame | list[dict[str, Any]]
         self._metadata: dict[str, dict[str, list[Any]]] = {}
         match pseudo_response:
             case PseudoFieldResponse(dataframe, raw_metadata):
                 self._pseudo_data = dataframe
 
                 datadoc_fields: list[PseudoVariable] = []
+                datadoc_paths: list[str | None] = []
 
                 for field_metadata in raw_metadata:
                     pseudo_variable = self._datadoc_from_raw_metadata_fields(
                         field_metadata.datadoc
                     )
-                    if pseudo_variable is not None:
+                    if (
+                        pseudo_variable is not None
+                        and pseudo_variable.data_element_path not in datadoc_paths
+                    ):
+                        datadoc_paths.append(pseudo_variable.data_element_path)
                         datadoc_fields.append(pseudo_variable)
 
                     if field_metadata.field_name is None:
                         field_metadata.field_name = "unknown_field"
 
+                    # Add metadata per field
                     self._metadata[field_metadata.field_name] = {
                         "logs": field_metadata.logs,
                         "metrics": field_metadata.metrics,
                     }
 
                 self._datadoc = MetadataContainer(
                     pseudonymization=PseudonymizationMetadata(
@@ -73,15 +80,15 @@
                 )
                 self._datadoc = MetadataContainer(
                     pseudonymization=PseudonymizationMetadata(
                         pseudo_variables=pseudo_variables
                     )
                 )
 
-    def to_polars(self, **kwargs: t.Any) -> pl.DataFrame:
+    def to_polars(self, **kwargs: Any) -> pl.DataFrame:
         """Output pseudonymized data as a Polars DataFrame.
 
         Args:
             **kwargs: Additional keyword arguments to be passed the Polars "from_dicts" function *if* the input data is from a file.
 
         Raises:
             ValueError: If the result is not of type Polars DataFrame or PseudoFileResponse.
@@ -97,15 +104,15 @@
                 return df
             case list() as file_data:
                 df = pl.from_dicts(file_data, **kwargs)
                 return df
             case _ as invalid_pseudo_data:
                 raise ValueError(f"Invalid file type: {type(invalid_pseudo_data)}")
 
-    def to_pandas(self, **kwargs: t.Any) -> pd.DataFrame:
+    def to_pandas(self, **kwargs: Any) -> pd.DataFrame:
         """Output pseudonymized data as a Pandas DataFrame.
 
         Args:
             **kwargs: Additional keyword arguments to be passed the Pandas reader function *if* the input data is from a file.
                 The specific reader function depends on the format of the input file, e.g. `read_csv()` for CSV files.
 
         Raises:
@@ -118,15 +125,15 @@
             case pl.DataFrame() as df:
                 return df.to_pandas()
             case list() as file_data:
                 return pd.DataFrame.from_records(file_data, **kwargs)
             case _ as invalid_pseudo_data:
                 raise ValueError(f"Invalid response type: {type(invalid_pseudo_data)}")
 
-    def to_file(self, file_path: str, **kwargs: t.Any) -> None:
+    def to_file(self, file_path: str, **kwargs: Any) -> None:
         """Write pseudonymized data to a file, with the metadata being written to the same folder.
 
         Args:
             file_path (str): The path to the file to be written. If writing to a bucket, use the "gs://" prefix.
             **kwargs: Additional keyword arguments to be passed the Polars writer function *if* the input data is a DataFrame.
                 The specific writer function depends on the format of the output file, e.g. `write_csv()` for CSV files.
 
@@ -150,15 +157,15 @@
             datadoc_file_handle = datadoc_file_path.open(mode="w")
         else:
             file_handle = Path(file_path).open(mode="wb")
 
             datadoc_file_path = Path(file_path).parent.joinpath(Path(datadoc_file_name))
             datadoc_file_handle = datadoc_file_path.open(mode="w")
 
-        file_handle = t.cast(
+        file_handle = cast(
             BufferedWriter, file_handle
         )  # file handle is always BufferedWriter when opening with "wb"
 
         match self._pseudo_data:
             case pl.DataFrame() as df:
                 write_from_df(df, file_format, file_handle, **kwargs)
                 datadoc_file_handle.write(self.datadoc)
@@ -170,25 +177,36 @@
             case _ as invalid_pseudo_data:
                 raise ValueError(f"Invalid response type: {type(invalid_pseudo_data)}")
 
         file_handle.close()
         datadoc_file_handle.close()
 
     @property
-    def metadata(self) -> dict[str, Any]:
-        """Returns the pseudonymization metadata as a dictionary.
+    def metadata_details(self) -> dict[str, Any]:
+        """Returns the pseudonymization metadata as a dictionary, for each field that has been processed.
 
         Returns:
             Optional[dict[str, str]]: A dictionary containing the pseudonymization metadata,
             where the keys are field names and the values are corresponding pseudo field metadata.
             If no metadata is set, returns an empty dictionary.
         """
         return self._metadata
 
     @property
+    def metadata(self) -> dict[str, Any]:
+        """Returns the aggregated metadata for all fields as a dictionary.
+
+        Returns:
+            Optional[dict[str, str]]: A dictionary containing the pseudonymization metadata,
+            where the keys are field names and the values are corresponding pseudo field metadata.
+            If no metadata is set, returns an empty dictionary.
+        """
+        return aggregate_metrics(self._metadata)
+
+    @property
     def datadoc(self) -> str:
         """Returns the pseudonymization metadata as a dictionary.
 
         Returns:
             str: A JSON-formattted string representing the datadoc metadata.
         """
         return self._datadoc.model_dump_json(exclude_none=True)
@@ -198,7 +216,28 @@
         raw_metadata: list[dict[str, Any]],
     ) -> PseudoVariable | None:
         if len(raw_metadata) == 0:
             return None
         elif len(raw_metadata) > 1:
             print(f"Unexpected length of metadata: {len(raw_metadata)}")
         return PseudoVariable.model_validate(raw_metadata[0])
+
+
+def aggregate_metrics(metadata: dict[str, dict[str, list[Any]]]) -> dict[str, Any]:
+    """Aggregates logs and metrics. Each unique metric is summarized."""
+    logs: list[str] = []
+    metrics: Counter[str] = Counter()
+    for field_metadata in metadata.values():
+        for metadata_field, metadata_value in field_metadata.items():
+            match metadata_field:
+                case "logs":
+                    # Logs are simply appended
+                    logs.extend(metadata_value)
+                case "metrics":
+                    # Count each unique metric
+                    metadata_value = cast(list[dict[str, int]], metadata_value)
+                    # Metrics is represented by a list of dicts, e.g. [{"METRIC_1": 1}, {"METRIC_2": 1}]
+                    for metric in metadata_value:
+                        # Each dict has a single entry, e.g. {"METRIC_1": 1}, so take the first one
+                        key, value = next(iter(metric.items()))
+                        metrics.update({key: value})
+    return {"logs": logs, "metrics": dict(metrics)}
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/validation.py` & `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import pandas as pd
 import polars as pl
 import requests
 
 from dapla_pseudo.utils import convert_to_date
 from dapla_pseudo.utils import get_file_format_from_file_name
 from dapla_pseudo.v1.client import _client
-from dapla_pseudo.v1.pseudo_commons import PseudoFieldResponse
-from dapla_pseudo.v1.pseudo_commons import RawPseudoMetadata
+from dapla_pseudo.v1.models.api import PseudoFieldResponse
+from dapla_pseudo.v1.models.api import RawPseudoMetadata
 from dapla_pseudo.v1.result import Result
 from dapla_pseudo.v1.supported_file_format import read_to_polars_df
 
 
 class Validator:
     """Starting point for validation of datasets.
```

### Comparing `dapla_toolbelt_pseudo-1.8.6/PKG-INFO` & `dapla_toolbelt_pseudo-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 1.8.6
+Version: 2.0.0
 Summary: Pseudonymization extensions for Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Dapla Developers
 Author-email: dapla-platform-developers@ssb.no
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -14,24 +14,26 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: cloudpathlib[gs] (>=0.17.0)
 Requires-Dist: cryptography (>41.0.0)
 Requires-Dist: dapla-toolbelt (>=1.7.0)
 Requires-Dist: fsspec (>=2023.5.0)
+Requires-Dist: orjson (>=3.10.1,<4.0.0)
 Requires-Dist: pandas-stubs (>=1.5.3.230304)
 Requires-Dist: polars (>=0.18.2)
 Requires-Dist: puremagic (>=1.15)
 Requires-Dist: pyarrow (>=14.0.2,<15)
 Requires-Dist: pydantic (>=2.0)
 Requires-Dist: pygments (>2.15.0)
 Requires-Dist: pyhumps (>=3.8.0)
 Requires-Dist: python-ulid (>=2.2.0)
 Requires-Dist: ssb-datadoc-model (>=5.0.0)
 Requires-Dist: types-requests (>=2.28.11)
+Requires-Dist: wcmatch (>=8.5.1,<9.0.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/dapla-toolbelt-pseudo/releases
 Project-URL: Documentation, https://statisticsnorway.github.io/dapla-toolbelt-pseudo
 Project-URL: Repository, https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 Description-Content-Type: text/markdown
 
 # Dapla Toolbelt Pseudo
 
@@ -299,15 +301,15 @@
      'func': 'redact(placeholder=#)' # This is a shorthand representation of the redact function
 }
 
 rule = PseudoRule.from_json(rule_json)
 
 df = (
     Pseudonymize.from_polars(df)
-    .add_rules(rule) # Add one or more pseudonymization rules
+    .add_rules(rule) # Add to pseudonymization rules
     .run()
     .to_polars()
 )
 ```
 
 Pseudonymization rules can also be read from file. This is especially handy when there are several rules, or if you
 prefer to store and maintain pseudonymization rules externally. For example:
```

