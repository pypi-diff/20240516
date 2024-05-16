# Comparing `tmp/bolt11-2.0.5.tar.gz` & `tmp/bolt11-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolt11-2.0.5.tar", max compression
+gzip compressed data, was "bolt11-2.0.6.tar", max compression
```

## Comparing `bolt11-2.0.5.tar` & `bolt11-2.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1112 2023-08-25 09:39:45.217153 bolt11-2.0.5/LICENSE
--rwxr-xr-x   0        0        0     3566 2023-08-25 09:39:45.221153 bolt11-2.0.5/README.md
--rw-r--r--   0        0        0      740 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/__init__.py
--rw-r--r--   0        0        0     1111 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/bit_utils.py
--rw-r--r--   0        0        0     2750 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/cli.py
--rw-r--r--   0        0        0      243 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/compat.py
--rw-r--r--   0        0        0     5351 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/decode.py
--rw-r--r--   0        0        0     3517 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/encode.py
--rw-r--r--   0        0        0     2993 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/exceptions.py
--rw-r--r--   0        0        0     2848 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/models/fallback.py
--rw-r--r--   0        0        0     4366 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/models/features.py
--rw-r--r--   0        0        0     1559 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/models/routehint.py
--rw-r--r--   0        0        0     2402 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/models/signature.py
--rw-r--r--   0        0        0     2310 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/models/tags.py
--rw-r--r--   0        0        0       26 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/py.typed
--rw-r--r--   0        0        0     5596 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/types.py
--rw-r--r--   0        0        0     2336 2023-08-25 09:39:45.221153 bolt11-2.0.5/bolt11/utils.py
--rw-r--r--   0        0        0     2095 2023-08-25 09:39:45.221153 bolt11-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     4304 1970-01-01 00:00:00.000000 bolt11-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1112 2024-05-16 07:34:43.126598 bolt11-2.0.6/LICENSE
+-rwxr-xr-x   0        0        0     3548 2024-05-16 07:34:43.126598 bolt11-2.0.6/README.md
+-rw-r--r--   0        0        0      740 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/__init__.py
+-rw-r--r--   0        0        0     1111 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/bit_utils.py
+-rw-r--r--   0        0        0     2750 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/cli.py
+-rw-r--r--   0        0        0      243 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/compat.py
+-rw-r--r--   0        0        0     5351 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/decode.py
+-rw-r--r--   0        0        0     3517 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/encode.py
+-rw-r--r--   0        0        0     2993 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/exceptions.py
+-rw-r--r--   0        0        0     2848 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/models/fallback.py
+-rw-r--r--   0        0        0     4366 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/models/features.py
+-rw-r--r--   0        0        0     1559 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/models/routehint.py
+-rw-r--r--   0        0        0     2402 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/models/signature.py
+-rw-r--r--   0        0        0     2310 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/models/tags.py
+-rw-r--r--   0        0        0       26 2024-05-16 07:34:43.126598 bolt11-2.0.6/bolt11/py.typed
+-rw-r--r--   0        0        0     5801 2024-05-16 07:34:43.130598 bolt11-2.0.6/bolt11/types.py
+-rw-r--r--   0        0        0     2343 2024-05-16 07:34:43.130598 bolt11-2.0.6/bolt11/utils.py
+-rw-r--r--   0        0        0     2145 2024-05-16 07:34:43.130598 bolt11-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4337 1970-01-01 00:00:00.000000 bolt11-2.0.6/PKG-INFO
```

### Comparing `bolt11-2.0.5/LICENSE` & `bolt11-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/README.md` & `bolt11-2.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -104,13 +104,11 @@
 
 ### running CLI encode
 ```
 $ poetry run bolt11 encode '{
   "currency": "bc",
   "amount_msat": 1000,
   "date": 1590000000,
-  "tags": {
-      "payment_hash": "0001020304050607080900010203040506070809000102030405060708090102",
-      "payment_secret": "1111111111111111111111111111111111111111111111111111111111111111",
-      "d": "description"
-  }
+  "payment_hash": "0001020304050607080900010203040506070809000102030405060708090102",
+  "payment_secret": "1111111111111111111111111111111111111111111111111111111111111111",
+  "description": "description"
 }' e126f68f7eafcc8b74f54d269fe206be715000f94dac067d1c04a8ca3b2db734
```

### Comparing `bolt11-2.0.5/bolt11/__init__.py` & `bolt11-2.0.6/bolt11/__init__.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/bit_utils.py` & `bolt11-2.0.6/bolt11/bit_utils.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/cli.py` & `bolt11-2.0.6/bolt11/cli.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/decode.py` & `bolt11-2.0.6/bolt11/decode.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/encode.py` & `bolt11-2.0.6/bolt11/encode.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/exceptions.py` & `bolt11-2.0.6/bolt11/exceptions.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/models/fallback.py` & `bolt11-2.0.6/bolt11/models/fallback.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/models/features.py` & `bolt11-2.0.6/bolt11/models/features.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/models/routehint.py` & `bolt11-2.0.6/bolt11/models/routehint.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/models/signature.py` & `bolt11-2.0.6/bolt11/models/signature.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/models/tags.py` & `bolt11-2.0.6/bolt11/models/tags.py`

 * *Files identical despite different names*

### Comparing `bolt11-2.0.5/bolt11/types.py` & `bolt11-2.0.6/bolt11/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,15 @@
     Bolt11NoPaymentSecretException,
     Bolt11NoSignatureException,
 )
 from .models.fallback import Fallback
 from .models.features import Features
 from .models.routehint import RouteHint
 from .models.signature import Signature
-from .models.tags import (
-    Tag,  # noqa: F401, F403
-    TagChar,
-    Tags,
-)
+from .models.tags import TagChar, Tags
 
 
 class MilliSatoshi(int):
     """A thousandth of a satoshi."""
 
     @classmethod
     def from_btc(cls, btc: Decimal) -> "MilliSatoshi":
@@ -63,16 +59,14 @@
             and self.tags.get(TagChar.description_hash)
             or not self.tags.get(TagChar.description)
             and not self.tags.get(TagChar.description_hash)
         ):
             raise Bolt11DescriptionException()
 
     def has_expired(self) -> bool:
-        if self.expiry is None:
-            return False
         return time.time() > self.date + self.expiry
 
     def is_mainnet(self) -> bool:
         return self.currency == "bc"
 
     def is_testnet(self) -> bool:
         return self.currency == "tb"
@@ -94,22 +88,37 @@
         return tag.data if tag else None
 
     @property
     def metadata(self) -> Optional[str]:
         tag = self.tags.get(TagChar.metadata)
         return tag.data if tag else None
 
+    # backwards compatibility
     @property
     def dt(self) -> datetime:
+        return self.date_time
+
+    @property
+    def date_time(self) -> datetime:
         return datetime.fromtimestamp(self.date)
 
     @property
-    def expiry(self) -> Optional[int]:
+    def expiry(self) -> int:
         tag = self.tags.get(TagChar.expire_time)
-        return tag.data if tag else None
+        if not tag:
+            return 3600
+        return tag.data
+
+    @property
+    def expiry_date(self) -> datetime:
+        return datetime.fromtimestamp(self.date + self.expiry)
+
+    @property
+    def expiry_time(self) -> int:
+        return self.date + self.expiry
 
     @property
     def features(self) -> Optional[Features]:
         tag = self.tags.get(TagChar.features)
         return tag.data if tag else None
 
     @property
@@ -150,27 +159,26 @@
     @property
     def data(self) -> dict:
         data = {
             "currency": self.currency,
             "amount_msat": int(self.amount_msat) if self.amount_msat else 0,
             "date": self.date,
             "signature": self.signature.hex if self.signature else "",
+            "expiry": self.expiry,
         }
         if self.has_payment_hash:
             data["payment_hash"] = self.payment_hash
         if self.payment_secret:
             data["payment_secret"] = self.payment_secret
         if self.description:
             data["description"] = self.description
         if self.description_hash:
             data["description_hash"] = self.description_hash
         if self.metadata:
             data["metadata"] = self.metadata
-        if self.expiry:
-            data["expiry"] = self.expiry
         if self.features:
             data["features"] = self.features.readable
         if self.fallback:
             data["fallback"] = self.fallback.address
         if self.route_hints:
             data["route_hints"] = [
                 [route._asdict() for route in route_hint.routes]
```

### Comparing `bolt11-2.0.5/bolt11/utils.py` & `bolt11-2.0.6/bolt11/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from decimal import Decimal
 from re import fullmatch, match
-from typing import Optional, Union
+from typing import Optional, Tuple, Union
 
 from .exceptions import Bolt11AmountInvalidException, Bolt11HrpInvalidException
 from .types import MilliSatoshi
 
 
-def verify_hrp(hrp: str) -> tuple[str, Optional[MilliSatoshi]]:
+def verify_hrp(hrp: str) -> Tuple[str, Optional[MilliSatoshi]]:
     matches = match(r"ln(bcrt|bc|tbs|tb)(\w+)?", hrp)
     if matches is None:
         raise Bolt11HrpInvalidException()
     currency, amount_str = matches.groups()
     return currency, amount_to_msat(amount_str) if amount_str else None
```

### Comparing `bolt11-2.0.5/pyproject.toml` & `bolt11-2.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bolt11"
-version = "2.0.5"
+version = "2.0.6"
 description = "A library for encoding and decoding BOLT11 payment requests."
 repository = "https://github.com/lnbits/bolt11"
 authors = [
     "eillarra <eneko@illarra.com>",
     "Alan Bits <alan@lnbits.com>"
 ]
 license = "MIT"
@@ -26,18 +26,18 @@
 ecdsa = "*"
 secp256k1 = "*"
 bech32 = "*"
 bitstring = "*"
 
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
+black = ">=23.7,<25.0"
 mypy = "^1.5.1"
 pytest = "^7.2.1"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 pyright = "^1.1.323"
 pre-commit = "^3.3.3"
 ruff = "^0.0.283"
 
 
 [build-system]
 requires = ["poetry-core"]
@@ -46,14 +46,15 @@
 
 [tool.mypy]
 ignore_missing_imports = "True"
 files = "bolt11"
 
 
 [tool.pytest.ini_options]
+addopts = "-s --cov=bolt11 --cov-report=xml"
 testpaths = [
   "tests"
 ]
 
 
 [tool.pyright]
 reportMissingImports = false
```

### Comparing `bolt11-2.0.5/PKG-INFO` & `bolt11-2.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: bolt11
-Version: 2.0.5
+Version: 2.0.6
 Summary: A library for encoding and decoding BOLT11 payment requests.
 Home-page: https://github.com/lnbits/bolt11
 License: MIT
 Author: eillarra
 Author-email: eneko@illarra.com
 Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: base58
 Requires-Dist: bech32
 Requires-Dist: bitstring
 Requires-Dist: click
 Requires-Dist: ecdsa
 Requires-Dist: secp256k1
 Project-URL: Repository, https://github.com/lnbits/bolt11
@@ -127,14 +128,12 @@
 
 ### running CLI encode
 ```
 $ poetry run bolt11 encode '{
   "currency": "bc",
   "amount_msat": 1000,
   "date": 1590000000,
-  "tags": {
-      "payment_hash": "0001020304050607080900010203040506070809000102030405060708090102",
-      "payment_secret": "1111111111111111111111111111111111111111111111111111111111111111",
-      "d": "description"
-  }
+  "payment_hash": "0001020304050607080900010203040506070809000102030405060708090102",
+  "payment_secret": "1111111111111111111111111111111111111111111111111111111111111111",
+  "description": "description"
 }' e126f68f7eafcc8b74f54d269fe206be715000f94dac067d1c04a8ca3b2db734
```

