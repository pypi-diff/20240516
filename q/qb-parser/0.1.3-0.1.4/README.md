# Comparing `tmp/qb_parser-0.1.3.tar.gz` & `tmp/qb_parser-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qb_parser-0.1.3.tar", max compression
+gzip compressed data, was "qb_parser-0.1.4.tar", max compression
```

## Comparing `qb_parser-0.1.3.tar` & `qb_parser-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2819 2024-05-13 03:26:41.423969 qb_parser-0.1.3/README.md
--rw-r--r--   0        0        0      275 2024-05-16 03:26:21.767199 qb_parser-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      130 2024-05-16 03:26:14.505342 qb_parser-0.1.3/qb_parser/__init__.py
--rw-r--r--   0        0        0     8243 2024-05-13 03:20:33.474044 qb_parser-0.1.3/qb_parser/answerline_parser.py
--rw-r--r--   0        0        0     3430 2024-05-13 03:28:50.913941 qb_parser-0.1.3/qb_parser/clue_tokenizer.py
--rw-r--r--   0        0        0     2920 2024-05-12 23:05:57.017276 qb_parser-0.1.3/qb_parser/util.py
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 qb_parser-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2819 2024-05-13 03:26:41.423969 qb_parser-0.1.4/README.md
+-rw-r--r--   0        0        0      275 2024-05-16 03:35:18.875767 qb_parser-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-16 03:28:46.544202 qb_parser-0.1.4/qb_parser/__init__.py
+-rw-r--r--   0        0        0     8244 2024-05-16 03:35:13.014351 qb_parser-0.1.4/qb_parser/answerline_parser.py
+-rw-r--r--   0        0        0     3430 2024-05-13 03:28:50.913941 qb_parser-0.1.4/qb_parser/clue_tokenizer.py
+-rw-r--r--   0        0        0     2920 2024-05-12 23:05:57.017276 qb_parser-0.1.4/qb_parser/util.py
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 qb_parser-0.1.4/PKG-INFO
```

### Comparing `qb_parser-0.1.3/README.md` & `qb_parser-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `qb_parser-0.1.3/qb_parser/answerline_parser.py` & `qb_parser-0.1.4/qb_parser/answerline_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from enum import  Enum
 from dataclasses import dataclass, field
 from typing import Dict, List, Tuple
 
-from util import *
+from .util import *
 
 class Directive(str, Enum):
     ACCEPT = "accept"
     REJECT = "reject"
     PROMPT = "prompt"
     REGULAR_PROMPT = "regular_prompt"
     ANTIPROMPT = "antiprompt"
```

### Comparing `qb_parser-0.1.3/qb_parser/clue_tokenizer.py` & `qb_parser-0.1.4/qb_parser/clue_tokenizer.py`

 * *Files identical despite different names*

### Comparing `qb_parser-0.1.3/qb_parser/util.py` & `qb_parser-0.1.4/qb_parser/util.py`

 * *Files identical despite different names*

### Comparing `qb_parser-0.1.3/PKG-INFO` & `qb_parser-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qb-parser
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: YichiRockyZhang
 Author-email: rocky1oo.zhang@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

