# Comparing `tmp/puppetparser-0.2.5.tar.gz` & `tmp/puppetparser-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puppetparser-0.2.5.tar", max compression
+gzip compressed data, was "puppetparser-0.2.6.tar", max compression
```

## Comparing `puppetparser-0.2.5.tar` & `puppetparser-0.2.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-01-03 13:45:14.417814 puppetparser-0.2.5/LICENSE
--rw-r--r--   0        0        0      804 2024-03-22 17:40:49.304234 puppetparser-0.2.5/README.md
--rw-r--r--   0        0        0       22 2024-01-03 13:45:14.417814 puppetparser-0.2.5/puppetparser/.gitignore
--rw-r--r--   0        0        0        0 2024-01-03 13:45:14.417814 puppetparser-0.2.5/puppetparser/__init__.py
--rw-r--r--   0        0        0       98 2024-03-22 19:57:57.298496 puppetparser-0.2.5/puppetparser/__main__.py
--rw-r--r--   0        0        0    11508 2024-03-23 12:11:46.688998 puppetparser-0.2.5/puppetparser/model.py
--rw-r--r--   0        0        0    64997 2024-05-07 14:12:37.072439 puppetparser-0.2.5/puppetparser/parser.py
--rw-r--r--   0        0        0     1001 2024-05-07 14:13:39.647548 puppetparser-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 puppetparser-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-01-03 13:45:14.417814 puppetparser-0.2.6/LICENSE
+-rw-r--r--   0        0        0      804 2024-03-22 17:40:49.304234 puppetparser-0.2.6/README.md
+-rw-r--r--   0        0        0       22 2024-01-03 13:45:14.417814 puppetparser-0.2.6/puppetparser/.gitignore
+-rw-r--r--   0        0        0        0 2024-01-03 13:45:14.417814 puppetparser-0.2.6/puppetparser/__init__.py
+-rw-r--r--   0        0        0       98 2024-03-22 19:57:57.298496 puppetparser-0.2.6/puppetparser/__main__.py
+-rw-r--r--   0        0        0    11729 2024-05-16 10:38:31.782853 puppetparser-0.2.6/puppetparser/model.py
+-rw-r--r--   0        0        0    64997 2024-05-07 14:12:37.072439 puppetparser-0.2.6/puppetparser/parser.py
+-rw-r--r--   0        0        0     1001 2024-05-16 10:38:54.050534 puppetparser-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 puppetparser-0.2.6/PKG-INFO
```

### Comparing `puppetparser-0.2.5/LICENSE` & `puppetparser-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.5/README.md` & `puppetparser-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.5/puppetparser/model.py` & `puppetparser-0.2.6/puppetparser/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
+from types import NoneType
 from typing import Dict, List, Tuple, Optional, Generic, TypeVar
 
-T = TypeVar("T")
+T = TypeVar(
+    "T",
+    str,
+    int,
+    float,
+    bool,
+    NoneType,
+    Dict["CodeElement", "CodeElement"],
+    List["CodeElement"],
+)
 
 
 class CodeElement:
     def __init__(self, line: int, col: int, end_line: int, end_col: int) -> None:
         self.line: int = line
         self.col: int = col
         self.end_line: int = end_line
@@ -23,15 +33,18 @@
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, self.__class__):
             return False
         return self.value == __o.value
 
     def __hash__(self) -> int:
-        return self.value.__hash__()
+        if self.value is None:
+            return 0
+
+        return self.value.__hash__()  # type: ignore
 
 
 class Hash(Value[Dict[CodeElement, CodeElement]]):
     def __init__(
         self,
         line: int,
         col: int,
```

### Comparing `puppetparser-0.2.5/puppetparser/parser.py` & `puppetparser-0.2.6/puppetparser/parser.py`

 * *Files identical despite different names*

### Comparing `puppetparser-0.2.5/pyproject.toml` & `puppetparser-0.2.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "puppetparser"
-version = "0.2.5"
+version = "0.2.6"
 description = "A parser from Puppet to an object model"
 authors = ["Nuno Saavedra <nuno.saavedra@tecnico.ulisboa.pt>"]
 license = "GPL-3.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `puppetparser-0.2.5/PKG-INFO` & `puppetparser-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puppetparser
-Version: 0.2.5
+Version: 0.2.6
 Summary: A parser from Puppet to an object model
 License: GPL-3.0
 Keywords: puppet,parser,object model
 Author: Nuno Saavedra
 Author-email: nuno.saavedra@tecnico.ulisboa.pt
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

