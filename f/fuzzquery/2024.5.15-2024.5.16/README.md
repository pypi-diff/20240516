# Comparing `tmp/fuzzquery-2024.5.15.tar.gz` & `tmp/fuzzquery-2024.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzquery-2024.5.15.tar", last modified: Thu May 16 03:36:00 2024, max compression
+gzip compressed data, was "fuzzquery-2024.5.16.tar", last modified: Thu May 16 17:37:50 2024, max compression
```

## Comparing `fuzzquery-2024.5.15.tar` & `fuzzquery-2024.5.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 03:36:00.505012 fuzzquery-2024.5.15/
--rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-2024.5.15/LICENSE
--rw-rw-rw-   0        0        0      692 2024-05-16 03:36:00.489387 fuzzquery-2024.5.15/PKG-INFO
--rw-rw-rw-   0        0        0       87 2024-05-16 01:41:23.000000 fuzzquery-2024.5.15/README.md
--rw-rw-rw-   0        0        0      692 2024-05-16 03:23:21.000000 fuzzquery-2024.5.15/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 03:36:00.505012 fuzzquery-2024.5.15/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 03:36:00.426882 fuzzquery-2024.5.15/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 03:36:00.458135 fuzzquery-2024.5.15/src/fuzzquery/
--rw-rw-rw-   0        0        0       21 2024-05-16 01:30:07.000000 fuzzquery-2024.5.15/src/fuzzquery/__init__.py
--rw-rw-rw-   0        0        0     4985 2024-05-16 00:11:55.000000 fuzzquery-2024.5.15/src/fuzzquery/main.py
-drwxrwxrwx   0        0        0        0 2024-05-16 03:36:00.489387 fuzzquery-2024.5.15/src/fuzzquery.egg-info/
--rw-rw-rw-   0        0        0      692 2024-05-16 03:36:00.000000 fuzzquery-2024.5.15/src/fuzzquery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2024-05-16 03:36:00.000000 fuzzquery-2024.5.15/src/fuzzquery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 03:36:00.000000 fuzzquery-2024.5.15/src/fuzzquery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 03:36:00.000000 fuzzquery-2024.5.15/src/fuzzquery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-16 03:36:00.000000 fuzzquery-2024.5.15/src/fuzzquery.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 17:37:50.707788 fuzzquery-2024.5.16/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-2024.5.16/LICENSE
+-rw-rw-rw-   0        0        0     6914 2024-05-16 17:37:50.707788 fuzzquery-2024.5.16/PKG-INFO
+-rw-rw-rw-   0        0        0     6311 2024-05-16 17:33:58.000000 fuzzquery-2024.5.16/README.md
+-rw-rw-rw-   0        0        0      692 2024-05-16 17:37:04.000000 fuzzquery-2024.5.16/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 17:37:50.707788 fuzzquery-2024.5.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 17:37:50.645286 fuzzquery-2024.5.16/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 17:37:50.676537 fuzzquery-2024.5.16/src/fuzzquery/
+-rw-rw-rw-   0        0        0       21 2024-05-16 01:30:07.000000 fuzzquery-2024.5.16/src/fuzzquery/__init__.py
+-rw-rw-rw-   0        0        0     4319 2024-05-16 17:36:21.000000 fuzzquery-2024.5.16/src/fuzzquery/main.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:37:50.707788 fuzzquery-2024.5.16/src/fuzzquery.egg-info/
+-rw-rw-rw-   0        0        0     6914 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 17:37:50.000000 fuzzquery-2024.5.16/src/fuzzquery.egg-info/top_level.txt
```

### Comparing `fuzzquery-2024.5.15/LICENSE` & `fuzzquery-2024.5.16/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzquery-2024.5.15/pyproject.toml` & `fuzzquery-2024.5.16/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fuzzquery"
-version = "2024.5.15"
+version = "2024.5.16"
 authors = [
   { name="OneMadGypsy", email="onemadgypsy@gmail.com" },
 ]
 description = "A lightwieght package for doing fuzzy matches with a simple query language"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fuzzquery-2024.5.15/src/fuzzquery/main.py` & `fuzzquery-2024.5.16/src/fuzzquery/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,21 @@
 import regex
 from   typing import Iterator
 
 __all__ = 'finditer', 'findany', 'iterall'
 
 REPL  = '`'                                  # character to represent substitution and deletion points
 TOKEN = regex.compile(r'\{(!{0,1}\d+|\?)\}') # for splitting on token guts
+FLAGS = regex.V1, regex.V1|regex.I           # case-sensitive, case-insensitive
 
 FORMAT = {# https://github.com/mrabarnett/mrab-regex?tab=readme-ov-file#approximate-fuzzy-matching-hg-issue-12-hg-issue-41-hg-issue-109
     '.':r'{{{over}i+1d+1s<={limit}:\S}}',    # suggestive range
     '!':r'{{{limit}<=s<={limit}:\S}}'   ,    # strict range
     '?':r'(\w+\W+)*?'                   ,}   # 0 or more unknown words 
-
-FLAGS  = {# lookup table for str to RegexFlag conversion
-    'a':regex.ASCII       , 
-    'f':regex.FULLCASE    , 
-    'i':regex.IGNORECASE  , 
-    'L':regex.LOCALE      , 
-    'm':regex.MULTILINE   , 
-    's':regex.DOTALL      , 
-    'u':regex.UNICODE     , 
-    'x':regex.VERBOSE     , 
-    'w':regex.WORD        ,
-    'b':regex.BESTMATCH   , 
-    'e':regex.ENHANCEMATCH, 
-    'p':regex.POSIX       , 
-    'r':regex.REVERSE     , 
-    '0':regex.VERSION0    , 
-    '1':regex.VERSION1    ,}
- 
-# convert str to flags
-def __str2flags(flags:str) -> regex.RegexFlag:
-    flags_ = regex.VERSION1 # default
     
-    for flag in filter(None, map(FLAGS.get, flags)):
-        flags_ |= flag
-        
-    return flags_
 
 # convert query to expression
 def __expr(query:str, group:bool=True) -> str:
 
     # convert term segment to expression
     def subexpr(segment:str) -> str:
         # assume this is a token and get alleged integer range
@@ -67,20 +43,20 @@
     # create final expression
     return f'{"("*grp}{expr}{")"*grp}'
    
 """ execute expression on text
     `expr` : final regex pattern
     `text` : the text to be searched
     `skip` : Iterable of words and/or characters that trigger a skip when found in a result - DEFAULT: []
-    `flags`: a string of regex flag characters                                              - DEFAULT: regex.VERSION1
+    `ci`   : case insensitive matching                                                      - DEFAULT: False
 """      
-def __exec(expr:str, text:str, skip:None|list|tuple|set=None, flags:str='') -> Iterator:
+def __exec(expr:str, text:str, skip:None|list|tuple|set=None, ci:bool=False) -> Iterator:
     skip = skip or []
     
-    for match in regex.finditer(expr, text, flags=__str2flags(flags)):
+    for match in regex.finditer(expr, text, flags=FLAGS[ci]):
         result = match['result']
         
         # determine if result should be skipped
         for item in skip:
             if item in result: break
         else:
             yield match.span(), result
```

