# Comparing `tmp/qb_parser-0.1.1.tar.gz` & `tmp/qb_parser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qb_parser-0.1.1.tar", max compression
+gzip compressed data, was "qb_parser-0.1.2.tar", max compression
```

## Comparing `qb_parser-0.1.1.tar` & `qb_parser-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2819 2024-05-13 03:26:41.423969 qb_parser-0.1.1/README.md
--rw-r--r--   0        0        0      275 2024-05-13 03:31:44.453904 qb_parser-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 01:01:03.261922 qb_parser-0.1.1/qb_parser/__init__.py
--rw-r--r--   0        0        0     8243 2024-05-13 03:20:33.474044 qb_parser-0.1.1/qb_parser/answerline_parser.py
--rw-r--r--   0        0        0     3430 2024-05-13 03:28:50.913941 qb_parser-0.1.1/qb_parser/clue_tokenizer.py
--rw-r--r--   0        0        0     2920 2024-05-12 23:05:57.017276 qb_parser-0.1.1/qb_parser/util.py
--rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 qb_parser-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2819 2024-05-13 03:26:41.423969 qb_parser-0.1.2/README.md
+-rw-r--r--   0        0        0      275 2024-05-16 03:19:36.465121 qb_parser-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       84 2024-05-16 03:19:28.224872 qb_parser-0.1.2/qb_parser/__init__.py
+-rw-r--r--   0        0        0     8243 2024-05-13 03:20:33.474044 qb_parser-0.1.2/qb_parser/answerline_parser.py
+-rw-r--r--   0        0        0     3430 2024-05-13 03:28:50.913941 qb_parser-0.1.2/qb_parser/clue_tokenizer.py
+-rw-r--r--   0        0        0     2920 2024-05-12 23:05:57.017276 qb_parser-0.1.2/qb_parser/util.py
+-rw-r--r--   0        0        0     3366 1970-01-01 00:00:00.000000 qb_parser-0.1.2/PKG-INFO
```

### Comparing `qb_parser-0.1.1/README.md` & `qb_parser-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qb_parser-0.1.1/qb_parser/answerline_parser.py` & `qb_parser-0.1.2/qb_parser/answerline_parser.py`

 * *Files identical despite different names*

### Comparing `qb_parser-0.1.1/qb_parser/clue_tokenizer.py` & `qb_parser-0.1.2/qb_parser/clue_tokenizer.py`

 * *Files identical despite different names*

### Comparing `qb_parser-0.1.1/qb_parser/util.py` & `qb_parser-0.1.2/qb_parser/util.py`

 * *Files identical despite different names*

### Comparing `qb_parser-0.1.1/PKG-INFO` & `qb_parser-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qb-parser
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: YichiRockyZhang
 Author-email: rocky1oo.zhang@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

