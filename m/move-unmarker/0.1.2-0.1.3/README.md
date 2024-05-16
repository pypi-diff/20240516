# Comparing `tmp/move_unmarker-0.1.2.tar.gz` & `tmp/move_unmarker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "move_unmarker-0.1.2.tar", max compression
+gzip compressed data, was "move_unmarker-0.1.3.tar", max compression
```

## Comparing `move_unmarker-0.1.2.tar` & `move_unmarker-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35823 2023-12-01 18:36:23.670955 move_unmarker-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2024-05-15 22:50:41.859290 move_unmarker-0.1.2/move_unmarker/__init__.py
--rw-r--r--   0        0        0     1023 2024-05-15 23:01:14.986025 move_unmarker-0.1.2/move_unmarker/unmarker.py
--rw-r--r--   0        0        0      612 2024-05-15 23:01:51.208119 move_unmarker-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1686 2024-05-15 23:01:05.196931 move_unmarker-0.1.2/README.md
--rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 move_unmarker-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-12-01 18:36:23.670955 move_unmarker-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-15 22:50:41.859290 move_unmarker-0.1.3/move_unmarker/__init__.py
+-rw-r--r--   0        0        0     1023 2024-05-15 23:01:14.986025 move_unmarker-0.1.3/move_unmarker/unmarker.py
+-rw-r--r--   0        0        0      612 2024-05-15 23:26:08.384629 move_unmarker-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1686 2024-05-15 23:25:42.074658 move_unmarker-0.1.3/README.md
+-rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 move_unmarker-0.1.3/PKG-INFO
```

### Comparing `move_unmarker-0.1.2/LICENSE` & `move_unmarker-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `move_unmarker-0.1.2/move_unmarker/unmarker.py` & `move_unmarker-0.1.3/move_unmarker/unmarker.py`

 * *Files identical despite different names*

### Comparing `move_unmarker-0.1.2/pyproject.toml` & `move_unmarker-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "move-unmarker"
-version = "0.1.2"
+version = "0.1.3"
 description = "CLI utility to remove PII watermarks from pdfs downloaded from Move USP/ESALQ"
 authors = ["João Fauvel <jmmfauvel@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/joaofauvel/move-unmarker"
 keywords = ["pdf", "watermark", "manipulation", "cli", "USP", "ESALQ"]
```

### Comparing `move_unmarker-0.1.2/README.md` & `move_unmarker-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     -o OUTPUT, --output OUTPUT
                             output filename (default: unmarked.pdf)
     -g GARBAGE, --garbage GARBAGE
                             level of garbage collection (default: 1)  
 [pymupdf.Document.save](https://pymupdf.readthedocs.io/en/latest/document.html#Document.save) method for more details on garbage collection.  
 
 ### TLDR
-- `unmarker watermarker.pdf`  
+- `unmarker watermarked.pdf`  
 - `unmarker -o unmarked.pdf watermarked.pdf`  
 - `unmarker --garbage 3 watermarked.pdf`
 
 ## Development
 1. Check Python's version `python -V`
 1. Install Python 3.8 or higher and pip, if they aren't already installed:
```

### Comparing `move_unmarker-0.1.2/PKG-INFO` & `move_unmarker-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: move-unmarker
-Version: 0.1.2
+Version: 0.1.3
 Summary: CLI utility to remove PII watermarks from pdfs downloaded from Move USP/ESALQ
 Home-page: https://github.com/joaofauvel/move-unmarker
 License: GPL-3.0-or-later
 Keywords: pdf,watermark,manipulation,cli,USP,ESALQ
 Author: João Fauvel
 Author-email: jmmfauvel@gmail.com
 Requires-Python: >=3.8
@@ -39,15 +39,15 @@
     -o OUTPUT, --output OUTPUT
                             output filename (default: unmarked.pdf)
     -g GARBAGE, --garbage GARBAGE
                             level of garbage collection (default: 1)  
 [pymupdf.Document.save](https://pymupdf.readthedocs.io/en/latest/document.html#Document.save) method for more details on garbage collection.  
 
 ### TLDR
-- `unmarker watermarker.pdf`  
+- `unmarker watermarked.pdf`  
 - `unmarker -o unmarked.pdf watermarked.pdf`  
 - `unmarker --garbage 3 watermarked.pdf`
 
 ## Development
 1. Check Python's version `python -V`
 1. Install Python 3.8 or higher and pip, if they aren't already installed:
```

