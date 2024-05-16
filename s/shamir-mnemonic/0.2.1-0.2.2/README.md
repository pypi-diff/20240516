# Comparing `tmp/shamir-mnemonic-0.2.1.tar.gz` & `tmp/shamir-mnemonic-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shamir-mnemonic-0.2.1.tar", last modified: Wed Feb  3 12:34:01 2021, max compression
+gzip compressed data, was "shamir-mnemonic-0.2.2.tar", last modified: Tue Dec  7 11:07:41 2021, max compression
```

## Comparing `shamir-mnemonic-0.2.1.tar` & `shamir-mnemonic-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2021-02-03 12:34:01.759603 shamir-mnemonic-0.2.1/
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1265 2021-02-03 12:26:06.000000 shamir-mnemonic-0.2.1/CHANGELOG.rst
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1051 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.1/LICENSE
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       38 2021-02-03 11:19:52.000000 shamir-mnemonic-0.2.1/MANIFEST.in
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     6155 2021-02-03 12:34:01.759603 shamir-mnemonic-0.2.1/PKG-INFO
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3089 2021-02-03 11:19:48.000000 shamir-mnemonic-0.2.1/README.rst
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      185 2021-02-03 12:34:01.763603 shamir-mnemonic-0.2.1/setup.cfg
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1081 2021-02-03 12:22:36.000000 shamir-mnemonic-0.2.1/setup.py
-drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2021-02-03 12:34:01.759603 shamir-mnemonic-0.2.1/shamir_mnemonic/
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      482 2021-02-03 11:19:48.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/__init__.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1949 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/cipher.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7334 2021-02-03 11:19:48.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/cli.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1659 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/constants.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3766 2021-02-03 11:19:48.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/recovery.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      929 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/rs1024.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    16175 2021-02-03 11:19:48.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/shamir.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     6186 2021-02-03 11:19:48.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/share.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1570 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/utils.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1113 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/wordlist.py
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7231 2019-03-28 13:16:18.000000 shamir-mnemonic-0.2.1/shamir_mnemonic/wordlist.txt
-drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2021-02-03 12:34:01.759603 shamir-mnemonic-0.2.1/shamir_mnemonic.egg-info/
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     6155 2021-02-03 12:34:01.000000 shamir-mnemonic-0.2.1/shamir_mnemonic.egg-info/PKG-INFO
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      592 2021-02-03 12:34:01.000000 shamir-mnemonic-0.2.1/shamir_mnemonic.egg-info/SOURCES.txt
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)        1 2021-02-03 12:34:01.000000 shamir-mnemonic-0.2.1/shamir_mnemonic.egg-info/dependency_links.txt
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       52 2021-02-03 12:34:01.000000 shamir-mnemonic-0.2.1/shamir_mnemonic.egg-info/entry_points.txt
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       27 2021-02-03 12:34:01.000000 shamir-mnemonic-0.2.1/shamir_mnemonic.egg-info/requires.txt
--rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       16 2021-02-03 12:34:01.000000 shamir-mnemonic-0.2.1/shamir_mnemonic.egg-info/top_level.txt
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2021-12-07 11:07:41.350992 shamir-mnemonic-0.2.2/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1513 2021-12-07 11:06:10.000000 shamir-mnemonic-0.2.2/CHANGELOG.rst
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1051 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.2/LICENSE
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       38 2021-02-03 11:19:52.000000 shamir-mnemonic-0.2.2/MANIFEST.in
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     6584 2021-12-07 11:07:41.350992 shamir-mnemonic-0.2.2/PKG-INFO
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3089 2021-02-03 11:19:48.000000 shamir-mnemonic-0.2.2/README.rst
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      256 2021-12-07 11:07:41.350992 shamir-mnemonic-0.2.2/setup.cfg
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1295 2021-12-07 11:06:10.000000 shamir-mnemonic-0.2.2/setup.py
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2021-12-07 11:07:41.350992 shamir-mnemonic-0.2.2/shamir_mnemonic/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      482 2021-02-03 11:19:48.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/__init__.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1949 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/cipher.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7189 2021-12-07 11:02:28.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/cli.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1659 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/constants.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     3755 2021-12-07 11:02:28.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/recovery.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      929 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/rs1024.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)    16175 2021-02-03 11:19:48.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/shamir.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     6235 2021-12-07 11:02:28.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/share.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1570 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/utils.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     1113 2021-01-12 10:31:45.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/wordlist.py
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     7231 2019-03-28 13:16:18.000000 shamir-mnemonic-0.2.2/shamir_mnemonic/wordlist.txt
+drwxrwxr-x   0 matejcik  (1000) matejcik  (1000)        0 2021-12-07 11:07:41.350992 shamir-mnemonic-0.2.2/shamir_mnemonic.egg-info/
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)     6584 2021-12-07 11:07:41.000000 shamir-mnemonic-0.2.2/shamir_mnemonic.egg-info/PKG-INFO
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)      592 2021-12-07 11:07:41.000000 shamir-mnemonic-0.2.2/shamir_mnemonic.egg-info/SOURCES.txt
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)        1 2021-12-07 11:07:41.000000 shamir-mnemonic-0.2.2/shamir_mnemonic.egg-info/dependency_links.txt
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       52 2021-12-07 11:07:41.000000 shamir-mnemonic-0.2.2/shamir_mnemonic.egg-info/entry_points.txt
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       69 2021-12-07 11:07:41.000000 shamir-mnemonic-0.2.2/shamir_mnemonic.egg-info/requires.txt
+-rw-rw-r--   0 matejcik  (1000) matejcik  (1000)       16 2021-12-07 11:07:41.000000 shamir-mnemonic-0.2.2/shamir_mnemonic.egg-info/top_level.txt
```

### Comparing `shamir-mnemonic-0.2.1/CHANGELOG.rst` & `shamir-mnemonic-0.2.2/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,28 @@
 `Semantic Versioning`_.
 
 `Unreleased`_
 -------------
 
 No changes yet
 
-.. _Unreleased: https://github.com/trezor/python-shamir-mnemonic/compare/v0.2.1...HEAD
+.. _Unreleased: https://github.com/trezor/python-shamir-mnemonic/compare/v0.2.2...HEAD
+
+
+`0.2.2`_ - 2021-12-07
+---------------------
+
+Changed
+~~~~~~~
+
+- Relaxed Click constraint so that Click 8.x is allowed
+- Applied `black` and `flake8` code style
+
+.. _0.2.2: https://github.com/trezor/python-shamir-mnemonic/compare/v0.2.1...v0.2.2
+
 
 `0.2.1`_ - 2021-02-03
 ---------------------
 
 .. _0.2.1: https://github.com/trezor/python-shamir-mnemonic/compare/v0.1.0...v0.2.1
 
 Fixed
```

### Comparing `shamir-mnemonic-0.2.1/LICENSE` & `shamir-mnemonic-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shamir-mnemonic-0.2.1/PKG-INFO` & `shamir-mnemonic-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: shamir-mnemonic
-Version: 0.2.1
+Version: 0.2.2
 Summary: SLIP-39 Shamir Mnemonics
 Home-page: https://github.com/trezor/python-shamir-mnemonic
 Author: Satoshi Labs
+Author-email: info@satoshilabs.com
 License: UNKNOWN
 Description: python-shamir-mnemonic
         ======================
         
         .. image:: https://badge.fury.io/py/shamir-mnemonic.svg
             :target: https://badge.fury.io/py/shamir-mnemonic
         
@@ -114,15 +115,28 @@
         `Semantic Versioning`_.
         
         `Unreleased`_
         -------------
         
         No changes yet
         
-        .. _Unreleased: https://github.com/trezor/python-shamir-mnemonic/compare/v0.2.1...HEAD
+        .. _Unreleased: https://github.com/trezor/python-shamir-mnemonic/compare/v0.2.2...HEAD
+        
+        
+        `0.2.2`_ - 2021-12-07
+        ---------------------
+        
+        Changed
+        ~~~~~~~
+        
+        - Relaxed Click constraint so that Click 8.x is allowed
+        - Applied `black` and `flake8` code style
+        
+        .. _0.2.2: https://github.com/trezor/python-shamir-mnemonic/compare/v0.2.1...v0.2.2
+        
         
         `0.2.1`_ - 2021-02-03
         ---------------------
         
         .. _0.2.1: https://github.com/trezor/python-shamir-mnemonic/compare/v0.1.0...v0.2.1
         
         Fixed
@@ -166,7 +180,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
+Provides-Extra: dev
+Provides-Extra: tests
```

### Comparing `shamir-mnemonic-0.2.1/README.rst` & `shamir-mnemonic-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `shamir-mnemonic-0.2.1/setup.py` & `shamir-mnemonic-0.2.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 from pathlib import Path
 
 from setuptools import setup
 
 # fmt: off
 REQUIREMENTS = [
     "attrs",
-    "click>=7,<8",
+    "click>=7,<9",
     "colorama",
 ]
+EXTRA_REQUIREMENTS = {
+    "dev": [
+        "black",
+        "flake8",
+        "isort"
+    ],
+    "tests": [
+        "pytest"
+    ]
+}
 # fmt: on
 
 CWD = Path(__file__).resolve().parent
 
 
 setup(
     name="shamir-mnemonic",
-    version="0.2.1",
+    version="0.2.2",
     description="SLIP-39 Shamir Mnemonics",
     long_description="\n".join(
         (
             (CWD / "README.rst").read_text(),
             (CWD / "CHANGELOG.rst").read_text(),
         )
     ),
     url="https://github.com/trezor/python-shamir-mnemonic",
     author="Satoshi Labs",
+    author_email="info@satoshilabs.com",
     packages=["shamir_mnemonic"],
     python_requires=">=3.6",
     install_requires=REQUIREMENTS,
+    extras_require=EXTRA_REQUIREMENTS,
     package_data={"shamir_mnemonic": ["wordlist.txt"]},
     entry_points={"console_scripts": ["shamir=shamir_mnemonic.cli:cli"]},
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/cipher.py` & `shamir-mnemonic-0.2.2/shamir_mnemonic/cipher.py`

 * *Files identical despite different names*

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/cli.py` & `shamir-mnemonic-0.2.2/shamir_mnemonic/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import secrets
 import sys
-from collections import defaultdict
-from typing import Dict, List, Optional, Sequence, Set, Tuple
+from typing import Sequence, Tuple
 
-import attr
 import click
 from click import style
 
-from .constants import GROUP_PREFIX_LENGTH_WORDS
 from .recovery import RecoveryState
-from .shamir import combine_mnemonics, generate_mnemonics
+from .shamir import generate_mnemonics
 from .share import Share
 from .utils import MnemonicError
 
 
 @click.group()
 def cli() -> None:
     pass
@@ -68,15 +65,15 @@
     """
     if passphrase and not master_secret:
         raise click.ClickException(
             "Only use passphrase in conjunction with an explicit master secret"
         )
 
     if (groups or group_threshold is not None) and scheme != "custom":
-        raise click.BadArgumentUsage(f"To use -g/-t, you must select 'custom' scheme.")
+        raise click.BadArgumentUsage("To use -g/-t, you must select 'custom' scheme.")
 
     if scheme == "single":
         group_threshold = 1
         groups = [(1, 1)]
     elif scheme == "master":
         group_threshold = 1
         groups = [(1, 1), (3, 5)]
@@ -105,15 +102,15 @@
         sys.exit(1)
 
     if master_secret is not None:
         try:
             secret_bytes = bytes.fromhex(master_secret)
         except Exception as e:
             raise click.BadOptionUsage(
-                "master_secret", f"Secret bytes must be hex encoded"
+                "master_secret", "Secret bytes must be hex encoded"
             ) from e
     else:
         secret_bytes = secrets.token_bytes(strength // 8)
 
     secret_hex = style(secret_bytes.hex(), bold=True)
     click.echo(f"Using master secret: {secret_hex}")
```

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/constants.py` & `shamir-mnemonic-0.2.2/shamir_mnemonic/constants.py`

 * *Files identical despite different names*

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/recovery.py` & `shamir-mnemonic-0.2.2/shamir_mnemonic/recovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections import defaultdict
-from typing import Any, Dict, List, Optional, Set, Tuple
+from typing import Any, Dict, Optional, Tuple
 
 import attr
 
 from .constants import GROUP_PREFIX_LENGTH_WORDS
 from .shamir import ShareGroup, recover_ems
 from .share import Share, ShareCommonParameters
 from .utils import MnemonicError
```

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/rs1024.py` & `shamir-mnemonic-0.2.2/shamir_mnemonic/rs1024.py`

 * *Files identical despite different names*

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/shamir.py` & `shamir-mnemonic-0.2.2/shamir_mnemonic/shamir.py`

 * *Files identical despite different names*

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/share.py` & `shamir-mnemonic-0.2.2/shamir_mnemonic/share.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,17 +146,21 @@
 
         identifier = id_exp_int >> ITERATION_EXP_LENGTH_BITS
         iteration_exponent = id_exp_int & ((1 << ITERATION_EXP_LENGTH_BITS) - 1)
 
         share_params_data = mnemonic_data[ID_EXP_LENGTH_WORDS : ID_EXP_LENGTH_WORDS + 2]
         share_params_int = _int_from_word_indices(share_params_data)
         share_params = int_to_indices(share_params_int, 5, 4)
-        group_index, group_threshold, group_count, index, member_threshold = (
-            share_params
-        )
+        (
+            group_index,
+            group_threshold,
+            group_count,
+            index,
+            member_threshold,
+        ) = share_params
 
         if group_count < group_threshold:
             raise MnemonicError(
                 'Invalid mnemonic "{} ...". Group threshold cannot be greater than group count.'.format(
                     " ".join(mnemonic.split()[: ID_EXP_LENGTH_WORDS + 2])
                 )
             )
```

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/utils.py` & `shamir-mnemonic-0.2.2/shamir_mnemonic/utils.py`

 * *Files identical despite different names*

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/wordlist.py` & `shamir-mnemonic-0.2.2/shamir_mnemonic/wordlist.py`

 * *Files identical despite different names*

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic/wordlist.txt` & `shamir-mnemonic-0.2.2/shamir_mnemonic/wordlist.txt`

 * *Files identical despite different names*

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic.egg-info/PKG-INFO` & `shamir-mnemonic-0.2.2/shamir_mnemonic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: shamir-mnemonic
-Version: 0.2.1
+Version: 0.2.2
 Summary: SLIP-39 Shamir Mnemonics
 Home-page: https://github.com/trezor/python-shamir-mnemonic
 Author: Satoshi Labs
+Author-email: info@satoshilabs.com
 License: UNKNOWN
 Description: python-shamir-mnemonic
         ======================
         
         .. image:: https://badge.fury.io/py/shamir-mnemonic.svg
             :target: https://badge.fury.io/py/shamir-mnemonic
         
@@ -114,15 +115,28 @@
         `Semantic Versioning`_.
         
         `Unreleased`_
         -------------
         
         No changes yet
         
-        .. _Unreleased: https://github.com/trezor/python-shamir-mnemonic/compare/v0.2.1...HEAD
+        .. _Unreleased: https://github.com/trezor/python-shamir-mnemonic/compare/v0.2.2...HEAD
+        
+        
+        `0.2.2`_ - 2021-12-07
+        ---------------------
+        
+        Changed
+        ~~~~~~~
+        
+        - Relaxed Click constraint so that Click 8.x is allowed
+        - Applied `black` and `flake8` code style
+        
+        .. _0.2.2: https://github.com/trezor/python-shamir-mnemonic/compare/v0.2.1...v0.2.2
+        
         
         `0.2.1`_ - 2021-02-03
         ---------------------
         
         .. _0.2.1: https://github.com/trezor/python-shamir-mnemonic/compare/v0.1.0...v0.2.1
         
         Fixed
@@ -166,7 +180,9 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.6
+Provides-Extra: dev
+Provides-Extra: tests
```

### Comparing `shamir-mnemonic-0.2.1/shamir_mnemonic.egg-info/SOURCES.txt` & `shamir-mnemonic-0.2.2/shamir_mnemonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

