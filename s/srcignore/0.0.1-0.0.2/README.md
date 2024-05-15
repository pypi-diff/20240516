# Comparing `tmp/srcignore-0.0.1.tar.gz` & `tmp/srcignore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srcignore-0.0.1.tar", max compression
+gzip compressed data, was "srcignore-0.0.2.tar", max compression
```

## Comparing `srcignore-0.0.1.tar` & `srcignore-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1058 2024-05-14 00:19:20.567064 srcignore-0.0.1/LICENSE
--rw-r--r--   0        0        0      178 2024-05-13 19:47:52.490650 srcignore-0.0.1/README.adoc
--rw-r--r--   0        0        0      708 2024-05-14 00:22:54.485969 srcignore-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 17:14:15.949327 srcignore-0.0.1/src/srcignore/__init__.py
--rw-r--r--   0        0        0     1079 2024-05-14 00:15:38.803780 srcignore-0.0.1/src/srcignore/main.py
--rw-r--r--   0        0        0        0 2024-05-13 21:17:17.408775 srcignore-0.0.1/src/srcignore/py.typed
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 srcignore-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-14 00:19:20.567064 srcignore-0.0.2/LICENSE
+-rw-r--r--   0        0        0      178 2024-05-13 19:47:52.490650 srcignore-0.0.2/README.adoc
+-rw-r--r--   0        0        0      708 2024-05-15 22:44:42.126554 srcignore-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 17:14:15.949327 srcignore-0.0.2/src/srcignore/__init__.py
+-rw-r--r--   0        0        0     1252 2024-05-15 22:49:55.279232 srcignore-0.0.2/src/srcignore/main.py
+-rw-r--r--   0        0        0        0 2024-05-13 21:17:17.408775 srcignore-0.0.2/src/srcignore/py.typed
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 srcignore-0.0.2/PKG-INFO
```

### Comparing `srcignore-0.0.1/LICENSE` & `srcignore-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `srcignore-0.0.1/pyproject.toml` & `srcignore-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "srcignore"
-version = "0.0.1"
+version = "0.0.2"
 description = "Generates a list of files that matches .gitignore-like files"
 authors = ["Calian AT"]
 readme = "README.adoc"
 homepage = "https://calian.com/"
 repository = "https://gitlab.com/brayden.willenborg/srcignore"
 license = "MIT"
 packages = [
```

### Comparing `srcignore-0.0.1/src/srcignore/main.py` & `srcignore-0.0.2/src/srcignore/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 
 import typer
 from gitignore_parser import parse_gitignore
 from typing_extensions import Annotated, List
 
 app = typer.Typer()
 
-def hi():
-    print(hi)
-
 @app.command()
 def ls(
     projectroot: Annotated[
         Path,
         typer.Argument(
             exists=True,
             file_okay=False,
@@ -34,19 +31,23 @@
             file_okay=True,
             dir_okay=False,
             writable=False,
             readable=True,
             resolve_path=True,
         ),
     ],
+    reverse: Annotated[bool, typer.Option()] = False
 ):
     matches = [ parse_gitignore(file) for file in ignore_files ]
 
     for filename in projectroot.rglob("*"):
         for match in matches:
-            if match(filename):
+            if match(filename) and not reverse:
+                print(filename.relative_to(projectroot))
+                break
+            elif not match(filename) and reverse:
                 print(filename.relative_to(projectroot))
                 break
 
 
 if __name__ == "__main__":  # pragma: no cover
     app()
```

### Comparing `srcignore-0.0.1/PKG-INFO` & `srcignore-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srcignore
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generates a list of files that matches .gitignore-like files
 Home-page: https://calian.com/
 License: MIT
 Author: Calian AT
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

